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

1.   To automatically construct the toolchain you need to make sure that you're
     in the `/home/glaucus` directory by running:

    ```Shell
    cd /home/glaucus
    ```

    Then execute the `run.sh` script located in the
    `/home/glaucus/scripts/toolchain` directory:

    ```Shell
    time dash /home/glaucus/scripts/toolchain/run.sh
    ```
