# 1.1. How to Build glaucus
glaucus will be built by using an already installed Linux distribution (such as
Arch Linux, Gentoo Linux, Void Linux, Fedora, or openSUSE). This existing Linux
system (the host) will be used as a starting point to provide necessary
programs, including a compiler, linker, and a shell, to build glaucus.

## 1.1.1. Chapter Two - Preparing the Host System
This chapter of the book describes how to prepare the host system for building
glaucus and what packages are required in order to do that.

## 1.1.2. Chapter Three - Cerata and Patches
This chapter explains which cerata (packages) and patches that need to be
fetched in order to build glaucus and how they're stored and handled.

## 1.1.3. Chapter Four - Final Preparations
Please read this chapter carefully as it explains several important issues you
need to be aware of before working your way through the rest of the chapters.

## 1.1.4. Chapter Five - Constructing the Toolchain
Explains how the cross and native toolchains, which are necessary to build
both the chroot environment and the final system glaucus, are constructed.

This chapter also shows you how to build a the first part of the toolchain which
is the cross toolchain, including the cross `binutils` and a slim version of
cross `gcc` that has been built without optimizations to further reduce build
times.

The cross toolchain is dynamically linked to the main C library of the
host system which is assumed to be `glibc`.

It further shows how the native toolchain is constructed by installing the
latest `linux-headers` followed by the `musl` libc which is going to be the
chroot's environment main C library. After that comes `libstdc++-v3` which is
needed to provide necessary C++ support to build the native toolchain. Then
comes the native binutils and gcc.

The native toolchain is dynamically linked to the chroot's environment main C
library which is `musl` and has nothing to do with the host's main C library
which is assumed to be `glibc`; thus achieving maximum isolation from the host
system.

## 1.1.5. Chapter Six - Constructing the Chroot Environment
Explains how the chroot environment is constructed using the native toolchain.
All cerata (packages) built in the chroot environment are dynamically linked to
the chroot's main C library which is `musl`.

When this chapter is done, glaucus's installation process will no longer depend
on the host system, with the exception of the running kernel.

This effort to isolate the new system from the host distribution may seem
excessive. A full technical explanation as to why this is done is provided in
Chapter 5, Section 2, titled “Toolchain Technical Notes”.

## 1.1.6. Chapter Seven - Installing Basic System Cerata
In this chapter the final system glaucus is built. The `chroot` program, which
stands for change root, is used to enter a virtual environment and start a new
`oksh` instance whose root directory will be set to the home directory of the
user glaucus.

This is very similar to rebooting and instructing the kernel to mount the home
directory of the user glaucus as the root partition. The system does not
actually reboot, but instead uses chroot because creating a bootable system
requires additional work which is not necessary just yet.

The major advantage is that *chrooting* allows you to continue using the host
system while the final system glaucus is being built. While waiting for cerata
compilations to complete, you can continue using your computer as normal.

## 1.1.7. Chapter Eight - System Configuration
The basic system configuration is set up in this chapter.

## 1.1.8. Chapter Nine - Making glaucus Bootable
The kernel and boot loader are set up in this chapter.

## 1.1.9. Chapter 10 - The End
Contains information on what to do after finishing the installation of glaucus.
