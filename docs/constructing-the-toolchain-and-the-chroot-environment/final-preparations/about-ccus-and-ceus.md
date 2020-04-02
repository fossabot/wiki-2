# 4.6. About CCUs and CEUs
Many people would like to know beforehand approximately how long it takes to
compile and install each package. Because glaucus can be built on many different
systems, it is impossible to provide accurate time estimates.

Instead of providing actual times, the Ceras Construct Unit (CCU) and the Ceras
Envenomate Unit (CEU) will measure the time required to prepare, configure,
build and install a ceras for both the toolchain and the chroot environment,
and the final system glaucus respectively.

!!! note
    When constructing the toolchain, cross `binutils` is given an CCU equivalent
    to 1, and the rest of the toolchain and chroot cerata are measured according
    to this CCU. Likewise, for the system cerata, the system `binutils` is given
    an CEU equivalent to 1, and the rest of the system cerata are measure
    according to this CEU.

For example, consider a package whose compilation time is 4.5 CCUs. This means
that if a system took 10 minutes to prepare, configure, build and install cross
`binutils`, then it'll take approximately 45 minutes to build this ceras.
Fortunately, most build times are shorter than the one for `binutils`.

!!! warning
    CCUs and CEUs are not entirely accurate because they depend on many factors,
    including the host system's version of `gcc` (for CCUs, when building the
    toolchain and the chroot environment). Keep in mind that the numbers can
    vary by as much as dozens of minutes in some cases.

!!! tip
    For many modern systems with multiple cores the compilation time for a ceras
    can be reduced by performing a "parallel `make`" by either setting an
    environment variable named `MAKEFLAGS` equal to the number of logical cores
    (or threads) on your host system or by telling the `make` program how many
    logical cores are available.

    Since glaucus is automated, the environment variable `MAKEFLAGS` is set in
    `/home/glaucus/scripts/flags` equal to `-j1` which is the sane default.

    To enable parallel building, you need to first know the number of threads on
    your host system. Simply run `nproc` and it'll return that number (let's say
    that `nproc` returned a value of `8`). Now you can set `MAKEFLAGS` to one of
    the following values:

    1.   `MAKEFLAGS=-j$(nproc)` which in our case is `MAKEFLAGS=-j8`:

         This sets the number of `MAKEFLAGS` equal to the number of the current
         threads on your host system. Some say that this will enable parallel
         building while giving some room for other applications to run as there
         will be an extra overhead thread that ensures your system doesn't lag
         or freeze.

    2.   `MAKEFLAGS=-j$(nproc + 1)` which in our case is `MAKEFLAGS=-j9`:

         This sets the number of `MAKEFLAGS` equal to the number of the current
         threads on your host system plus one. This is similar to the first
         option, but it ensures that the overhead thread is also used in the
         build process. This might build faster than option one, but will cause
         the system to lag a lot especially if you're using other applications
         such as a web browser.

    3.   `MAKEFLAGS=-j$(nproc * 1.5)` which in our case is `MAKEFLAGS=-j12`:

         Some say that in order for parallel building to work properly you need
         to set to set your `MAKEFLAGS` equal to the number of current threads
         times 1.5.

!!! warning
    glaucus doesn't enable parallel building by default, not because it's not
    supported but because it may sometimes result in some weird behaviour (e.g.
    scripts stop at preparation phase, or `install` giving warnings about
    attempts to create already existing directories) or even cause `make` to
    fail.

    Analyzing the output of the build process will also be more difficult
    because the lines of different threads will be interleaved. If you run into
    a problem with a build step, revert back to a single thread build
    (`MAKEFLAGS=-j1`) to properly analyze the error messages.
