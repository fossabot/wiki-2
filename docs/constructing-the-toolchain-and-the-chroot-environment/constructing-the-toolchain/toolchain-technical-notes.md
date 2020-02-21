# 5.2. Toolchain Technical Notes
This section explains some of the rationale and technical details behind the
overall construction method of the toolchain.

The overall goal of this Chapters 5 and 6 is to produce a temporary area that
contains a known-good set of tools that can be isolated from the host system. By
entering the chroot environment (using `chroot` of course, which is discussed in
the following chapter), the commands in the remaining chapters will be contained
within that environment, ensuring a clean, trouble-free build of the final
glaucus system.

This book has been designed to minimize the risks for new readers and to provide
the most educational value at the same time.

!!! note
    Before continuing, be aware of the name of the working platform, often
    referred to as the target tuple (which is often either a triplet or a
    quadruplet).

    A simple way to determine the name of the target triplet is to run
    `gcc -dumpmachine` and note the output. For example, for a 32-bit Intel
    processor the output will be i686-pc-linux-gnu, and on a 64-bit system it
    will be `x86_64-pc-linux-gnu` (that is if your host's main C library is
    Glibc).

    Also be aware of the name of the host's dynamic linker, often referred to as
    the dynamic loader (which is not to be confused with the standard linker
    `bfd` (aka regular `ld`) that is part of `binutils`). The dynamic linker
    provided by the host's C library (which is `glibc` in most cases) finds and
    loads the shared libraries needed by a program, prepares the program to run,
    and then runs it.

    For example, the dynamic linker for a 32-bit Intel machine would be
    `ld-linux.so.2`, and `ld-linux-x86-64.so.2` for 64-bit systems, both of
    which are located in either `/lib` or `/usr/lib`.

    A sure-fire way to determine the name of the dynamic linker is to inspect a
    random binary (e.g. `gcc`) from the host system by first locating where the
    binary is by running

    ```Shell
    which gcc
    ```
    
    then running:

    ```Shell
    readelf -l gcc | grep interpreter
    ```

    and noting the output, which will be similar to:

    ```Shell
    [Requesting program interpreter: /lib64/ld-linux-x86-64.so.2]
    ```

    on 64-bit systems.

!!! note
    The technically correct term to refer to a 64-bit system is `x86-64` and not
    `x86_64`. glaucus tries to use the former when and wherever possible but
    there are some cases/places where only the latter is recognized.

Some key technical points of how the toolchain is constructed:

1.   Slightly adjusting the name of the working platform, by changing the
     "vendor" field target tuple by way of the `$TUPL` environment variable
     which is automatically exported when running the
     `/home/glaucus/scripts/toolchain/run.sh`, ensures that both cross
     `binutils` and `gcc` produce a compatible cross-linker and cross-compiler.
     Instead of producing binaries for another architecture, the cross-linker
     and cross-compiler will produce binaries compatible with the current
     hardware.

2.   The toolchain libraries are cross-compiled, because a cross-compiler by its
     nature cannot rely on anything from its host system. This method removes
     potential contamination of the final system by lessening the chance of host
     headers or libraries being incorporated into system cerata.

3.   Careful manipulation of the `gcc` source tells the compiler which target
     dynamic linker will be used.

`binutils` is installed first because `gcc`'s configure script performs various
feature tests on the assembler and linker to determine which software features
to enable or disable. This is more important than one might first realize.

An incorrectly configured `gcc` or `musl` can result in a subtly broken
toolchain, where the impact of such breakage might not show up until near the
end of the build of an entire distribution. In most cases, a test suite failure
will usually highlight this error before too much additional work is performed.

`binutils` installs its assembler and linker in two locations, `$TOOL/bin` and
`$TOOL/$TUPL/bin`. The tools in one location are hard linked to the other. An
important facet of the linker is its library search order. Detailed information
can be obtained from `ld` by passing it the `--verbose` flag.

For example, an:

```Shell
ld --verbose | grep SEARCH
```

will illustrate the current search paths and their order. It shows which files
are linked by `ld` by compiling a dummy program and passing the `--verbose`
switch to the linker.

Another example is:

```Shell
gcc dummy.c -Wl,--verbose 2>&1 | grep succeeded
```

which will show all the files successfully opened during the linking.

The next ceras installed is `gcc`. An example of what can be seen during its
run of configure is:

```Shell
checking what assembler to use... /toolchain/x86_64-pc-linux-musl/bin/as
checking what linker to use... /toolchain/x86_64-pc-linux-musl/bin/ld
```

This is important for the reasons mentioned above. It also demonstrates that
`gcc`'s configure script does not search the `$PATH` directories to find which
utilities to use. However, during the actual operation of `gcc` itself, the same
search paths are not necessarily used. To find out which standard linker `gcc`
will use, run:

```Shell
gcc -print-prog-name=ld
```

Detailed information can be obtained from `gcc` by passing it the `-v` command line
option while compiling a dummy program. For example:

```Shell
gcc -v dummy.c
```

will show detailed information about the preprocessor, compilation, and assembly
stages, including `gcc`'s included search paths and their order.

Next installed are sanitized `linux-headers`. These allow the standard C library
(`musl`) to interface with features that the `linux` kernel will provide.

The next ceras installed is `musl`. The most important considerations for
building `musl` are `gcc`, `binutils` and `linux-headers`. The compiler
is generally not an issue since `musl` will always use the compiler relating to
the `$CROSS_COMPILE` variable; which in our case, compiler will be
`x86_64-pc-linux-musl-`.

During the native construction of `binutils`, we are able to utilize the
`--with-lib-path` configure switch to control `ld`'s library search path.

For the native construction of `gcc`, its sources also need to be modified to
tell `gcc` to use the new dynamic linker. Failure to do so will result in the
`gcc` programs themselves having the name of the dynamic linker from the host
system's `/usr/lib` (or `/lib`) directory embedded into them, which would defeat
the goal of getting away from the host.

From this point onwards, the toolchain is self-contained and self-hosted. Chroot
cerata belonging  will all be constructed against the new `musl` in `$TOOL`.

Upon entering the chroot environment, the first major ceras to be installed is
`musl`, due to its self-sufficient nature mentioned above. Once system `musl`is
installed into `/usr`, we will perform a quick adjustment of the toolchain
defaults, and then proceed in to envenomate the final system glaucus.
