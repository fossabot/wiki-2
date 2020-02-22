# 5.3. General Compilation Instructions
The basic instructions when compiling a ceras include:

*   The word ceras refers to a single package, while cerata refers to a group
    of packages.

*   There are four main stages to build glaucus and they are as follows:
    
    *    **cross** - which refers to the cross toolchain stage
    *    **native** - which refers to the native toolchain stage
    
    !!! note 
        The cross and native stages both are responsible for building the
        complete cross-native toolchain.

    *    **chroot** - which refers to the chroot environment
    *    **system** - which refers to the final system glaucus

*   The words compilation and build are often referred to as:
    
    *   **construct** - in the cross, native, chroot and system (before adjust is
        run ) stages

    *   **envenomate** - in the system stage (after adjust is run)

*   The scripts responsible for compiling the main stages are located in
    `/home/glaucus/scripts` and are as follows:

    *   **toolchain** - `/home/glaucus/scripts/toolchain/run.sh`

    !!! note
        As explained above, the toolchain `run.sh` will execute both `run.sh`
        scripts for cross and native.

    !!! warning
        Do not attempt to run `/home/glaucus/scripts/toolchain/cross/run.sh` or
        `/home/glaucus/scripts/toolchain/native/run.sh` alone as the latter
        requires the former to be constructed beforehand, and they both require
        a common set of environment variables only exported in the `variables`
        file `/home/glaucus/scripts/toolchain/variables` sourced by
        `/home/glaucus/scripts/toolchain/run.sh`.

    *   **chroot** - `/home/glaucus/scripts/chroot/run.sh`
    *   **system** - `/scripts/system/run.sh`

    !!! warning
        Remember you need to construct both the toolchain and the chroot
        environment (which will chroot you automatically) before running
        `/scripts/system/run.sh`.

*   The basic anatomy of any `run.sh` script is described below:

    *   All `run.sh` scripts start by sourcing a `variables` file located in
        their relative stages directories. The `variables` files are responsible
        for exporting several important environment flags that are used
        extensively in `$stage.ceras` files (where stage is cross, native,
        chroot or system).

    !!! note
        Notice how sourcing is done using the dot operator `.` for maximum
        compatibility instead of the word `source`, which is a synonym for the
        dot operator in BASH, but not in POSIX.

        Also notice how sourced scripts don't end with `.sh`. Only scripts that
        are manually called end with `.sh`.

    *  The `check` script comes next. This script is reponsible for fetching,
       verifying and extracting, or cloning cerata belonging to a particular
       stage.

    !!! note
        The only stage whose `check` script doesn't come after its `variables`
        script is the system stage, as we should already be inside the chroot
        environment which may not contain enough utilities needed to run the
        `check` script (even though `glaucus`'s chroot environment has a
        working internet connection).

        Instead the `check` script for the system stage is run just before
        entering the chroot environment.

        !!! note
            glaucus stores its ceras files, which contain instructions on how to
            build each ceras in every stage (be it cross, native, chroot or
            system) in the directory (/home/glaucus/cerata).

            The `check` stores the source files of glaucus cerata in the
            directory `/home/glaucus/sources`, where cerata that have version
            numbers other than `git` are stored as
            `/home/glaucus/sources/$ceras/$ceras-$ver` (where `$ceras` is the
            name of the ceras (e.g. `linux`) and `$ver` is its version (e.g.
            `5.5.5`) while its tarball is stored in
            `/home/glaucus/sources/$ceras`.

            Cerata that have versions equal to `git` (the `ver` variable in
            their `/home/glaucus/cerata/$ceras/ceras` files are equal to `git`)
            (e.g. Since there's no released version of `zlib-ng`, the check
            script will first check the `/home/glaucus/cerata/zlib-ng/ceras`
            file for the `ver` variable and see if it's equal to `git` (notice
            also how no `sum` variable exists in the `ceras` file of cerata that
            have `git` as their version) and clone its git repository to
            `/home/glaucus/sources/zlib-ng`.

    *   The following sourced script is generally the `prepare` script that
        perform some cleaning and preparation before `construct` or `envenomate`
        are run.

        For example, the toolchain's common `prepare` script ensures that both
        the `/home/glaucus/toolchain` directory and the `/toolchain` symlink are
        removed, then recreated with the symlink `/toolchain` pointing towards
        `/home/glaucus/toolchain`. It also creates another symlink
        `/toolchain/lib64` which points to `/toolchain/lib` (absolute path, it
        points to `lib` in the directory `/toolchain` to be more precise) to
        ensure the sanity of the toolchain.

        The `prepare` scripts for both **cross** and **native** ensure that the
        build directories `/temporary/toolchain/cross/builds` and
        `/temporary/toolchain/native/builds` are empty before the `construct`
        script is sourced.
    
    *  The following source script is `log` which executes the script passed to
       it as an argument while logging its stdout and stderr to an `out.log`
       file and an `err.log` file respectively in the directory
       `/home/glaucus/logs/$stage/$try` (where `$stage` is cross, native, chroot
       or system, and `$try` is the number of your current run; how many times
       you've attempted to run that script).

    !!! note
        In case a command fails, its exit status will be reported in a file
        called `exit` in `/home/glaucus/logs/$stage/$try` (where $stage is
        cross, native, chroot or system, and `$try` is the current number of
        your run; how many times you've attempted to run that script).

    !!! warning
        When a command fails the running script will automatically abort and
        return the exit status of the failing function along with the ceras
        (package) it failed at and at what function (prepare, configure,
        build or install) and in which stage (cross, native, chroot and
        system).  This will be displayed in the following format:

        !!! failure
            $stage $ceras $function exited with status $?

    *   The scripts passed to the sourced `log` script in `run.sh` as arguments
        are the `construct` and `envenomate` scripts. Both the `construct` and
        `envenomate` scripts share an identical structure so the only difference
        between the two is their names (and one technical minor difference which
        will be explained shortly):

        *   **construct** - is used to refer to the process of building
            something, or building the tools that will build something in the
            end. Since the toolchain, the chroot environment and the part of
            system before adjustment (system `linux-headers` and `musl`) are
            what build the final glaucus system (the part after adjustment), the
            word construct is used to refer to this process.

        *   **envenomate** - the use of this term stems from the fact the animal
            *Glaucus* consumes venemous creatures (e.g. *The Portuguese man o'
            war*) and concentrates their venom in sacs located at the tip of the
            animal's cerata. Similarly, glaucus builds its final system cerata
            by envenomating the `sac` directories (which are basically `DESTDIR`
            directories to keep track of installed files) producing `venom`
            directories containing both the final tarred archive and a `sum`
            file of its contents.

        !!! note
            The only technical difference between `construct` and `envenomate`
            is that envenomate uses directories called `sac`s as `DESTDIR`s to
            keep track of installed files since they're the final system cerata
            (packages).

        *   If we examine the content of a `construct` script or the
            `envenomate` script, we'll notice that a function with the name of
            the script is first defined (`construct()` for `construct`, and
            `envenomate()` for `envenomate`). This function takes only one
            argument (and creates the needed `sac` and `venom` directories for
            that one argument in the case of `envenomate`) and sources the
            `/home/glaucus/cerata/$ceras/ceras` file which contains all the
            required variables needed to construct or envenomate that ceras.

        !!! tip
            The use of the word ceras may get confusing at times, so to clear
            confusion:

            *   **ceras** - when mentioned alone it refers to the word package
            *   **ceras file** - the ceras file is a recipe file that only
                contains variables that provide information about a certain
                package, but doesn't contain functions or commands as it'll be
                commonly sourced in many stages so it has to be neutral
            *   **cerata** - refers to a group of packages or all of glaucus's
                packages
            *   **cerata directory** - refers to `/home/glaucus/cerata`
            *   **$stage.ceras** - files that contain the basic functions needed
                to build a package at a certain stage (cross, native, chroot or
                system).

            It then sources a `$stage.ceras` file which contains the basic four
            functions needed to build a ceras at a certain stageg (cross,
            native, chroot and system). The `$stage.ceras` files are located in
            `/home/glaucus/cerata/$ceras` and all consist of four main functions
            that regulate how a `construct` or `envenomate` process should be
            done. The four basic functions in all `$stage.ceras` files are as
            follows:

            1. **prepare_$stage()** - 
            2. **configure_$stage()** - 
            3. **build_$stage()** - 
            4. **install_$stage()** - 

*   Several cerata are patched before compilation patch is needed to circumvent
    a problem. A patch is often needed in both this and the next chapter, but
    sometimes in only one or the other.  Therefore, do not be concerned if
    instructions for a downloaded patch seem to be missing. Warning messages
    about offset or fuzz may also be encountered when applying a patch. Do not
    worry about these warnings, as the patch was still successfully applied.

During the compilation of most packages, there will be several warnings that
scroll by on the screen. These are normal and can safely be ignored. These
warnings are as they appear—warnings about deprecated, but not invalid, use of
the C or C++ syntax. C standards change fairly often, and some packages still
use the older standard. This is not a problem, but does prompt the warning.
