# 4.7. About the Test Suites
!!! note
    Support for testsuites hasn't been added to glaucus yet. It will be added in
    the future though, in the form of a function called `check_$stage()` (where
    stage is cross, native, chroot or system) for cerata that support
    testsuites.

Most cerata provide a test suite. Running the test suite for a newly built
package is a good idea because it can provide a “sanity check” indicating that
everything compiled correctly. A test suite that passes its set of checks
usually proves that the ceras is functioning as the developer intended. It does
not, however, guarantee that the ceras is totally bug free.

Some test suites are more important than others. For example, the test suites
for the cross and native toolchain cerata (`gcc` and `binutils`) are of utmost
importance due to their central role in a properly functioning system.

Running `gcc`'s testsuite is strongly recommended, even though it can take a
very long time to complete (especially on slower hardware).

!!! note
    Experience has shown that there is little to be gained from running
    testsuites for chroot cerata. There can be no escaping the fact that the
    host system always exerts some influence on the tests before entering the
    chroot environment (when building both the toolchain and the chroot
    environment itself), often causing inexplicable failures.

    Because the chroot environment will soon be replaced by the final system
    itself; the chroot environment is considered temporary and will eventually
    be discarded. Thus, we do not recommend running the test suites for chroot
    cerata for the average reader. The instructions for running those testsuites
    are provided for the benefit of testers and developers, but they are
    strictly optional.

A log section will be created in the future to gather the logs of both the
construct and envenomate processes as well as the testsuites to make it easier
to debug issues relating to them.
