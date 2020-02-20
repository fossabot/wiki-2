# 5.1. Introduction
This chapter shows how to build the main toolchain that'll be used on the host
system in order to build both the chroot environment and the final system
glaucus (with some adjustments to make it work inside the chroot environment,
until system gcc is built).

The chroot environment will contain just enough cerata to start constructing and
envenomating the final system glaucus in the Chapter 7. The chroot environment
is quite minimal and provides more convenience than a minimum environment would.

This chapter discusses how the new and host-independent toolchain, which uses
`gcc` as its compiler, `binutils`' `as` and `bfd` (or `ld`) as its assembler and
linker respectively, and `musl` as its C library) is constructed.

The files compiled in this chapter will be installed under the `$TOOL/`
directory to keep them separate from the files installed in the next chapter and
the host production directories. Since the cerata constructed here are
temporary, we do not want them to pollute the soon-to-be final system glaucus.
