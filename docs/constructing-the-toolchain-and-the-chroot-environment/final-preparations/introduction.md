# 4.1. Introduction
In this chapter, we will perform a few additional tasks to prepare for
constructing the toolchain and the chroot environment. A directory in `$GLAD`
will be created for the installation of the toolchain, add an unprivileged user
`glaucus` to reduce risk. An appropriate build environment for that user will
be created as well.

!!! note
    The unit of time used to measure how long glaucus cerata take to prepare,
    configure, build and install is referred to as “CCU” (Ceras Construct Unit)
    for toolchain and chroot cerata, and "CEU" (Ceras Envenomate Unit) for final
    system cerata. Both units will be provided in the future (they will probably
    be implemeted to be automatically measured).
