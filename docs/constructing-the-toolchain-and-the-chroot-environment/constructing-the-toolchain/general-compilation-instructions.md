# 5.3. General Compilation Instructions
The basic instructions when compiling a ceras include:

*   The word ceras refers to a single package, while cerata refers to a group
    of packages.

*   There are 4 main stages to build glaucus and they are as follows:
    
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

    *  The following source script is `log` which executes the script passed to
       it as an argument while logging its stdout and stderr to an `out.log`
       file and an `err.log` file respectively in the directory
       `/home/glaucus/logs/$stage/$try` (where $stage is cross, native, chroot
       or system, and `$try` is the number of your current run; how many times
       you've attempted to run that script).

       !!! note
           The exit status is reported in a file called `exit` in
           `/home/glaucus/logs/$stage/$try` (where $stage is cross, native,
           chroot or system, and `$try` is the number of your current run; how
           many times you've attempted to run that script).

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
