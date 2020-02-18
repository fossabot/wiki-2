# 3.1. Introduction
This chapter includes a list of cerata (packages) that are fetched automatically
in order to construct the toolchain, the chroot environment and the final system
glaucus.

The listed version numbers correspond to versions of the software that are known
to work, and this book is based on their use.

!!! warning
    We highly recommend against using newer versions because the build commands
    for one version may not work with a newer version. The newest package
    versions may also have problems that require work-arounds.

The `fetch` script (which is run automatically) will download all needed cerata
and the `check` script (which is also automatically run) will verify all
downloaded cerata, which will then be extracted (or cloned) to a subdirectory in
the sources directory.
