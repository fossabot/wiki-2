# 2.3. Building glaucus in Stages
glaucus is designed to be built in a single session; however, building it in
multiple sessions is also possible due to its automated nature (e.g. you can
build the toolchain in a single session, then build the chroot environment in
another).

!!! warning
    Constructing and envenomating the final system must be done in a single
    session. Exiting or terminating the `run` script of the final system will
    require some cleaning that will be explained in the near future.
