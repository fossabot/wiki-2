# v. Rationale for Cerata
## v.1. acl
Utilities to administer Access Control Lists.

## v.2. attr
Programs for administering extended attributes.

## v.3. autoconf
Programs for producing shell scripts that can automatically configure source
code from a developer's template.

## v.4. automake
Programs for generating Make files from a template.

## v.5. bash
The Bourne Again SHell is only included for compatibility purposes to provide
support for applications that have hardlinked paths to the bash executable
(mostly in the form of `/bin/bash`), and it's neither used as the main user
shell nor as the shell needed to build glaucus from scratch.

## v.6. bc
Gavin's implementation of the POSIX bc calculator with GNU extensions and dc,
which faster than GNU bc, and more POSIX compliant.

## v.7. binutils
A linker, an assembler, and other tools for handling object files.

## v.8. bison
The GNU version of yacc, included only for compatibility purposes to enable
cerata that require bison and only bison to build properly (e.g. the linux
kernel doesn't build with byacc).

## v.9. dash
A POSIX-compliant implementation of /bin/sh that aims to be as small as
possible. This is the main shell used for running scripts as all glaucus scripts
are written in POSIX DASH.

## v.10. diffutils
Programs that show the differences between files or directories.

## v.11. e2fsprogs
Utilities for handling the ext2, ext3 and ext4 file systems.

## v.12. elfutils-libelf
A DSO which allows reading and writing ELF files on a high level. This ceras
(package) only includes libelf from elfutils and not its entire utilities (which
may conflict with some binutils utilities, which is why the elfutils ceras
(package) has its utilities prefixed with the leters `eu-`)) and is required to
build the Linux kernel.

## v.13. eudev
A device manager.

## v.14. execline
A (non-interactive) scripting language, like sh ; but its syntax is quite
different from a traditional shell syntax. It's required to build s6-based
systems.

## v.15. expat
A relatively small XML parsing library.

## v.16. file
A utility for determining the type of a given file or files.

## v.17. findutils
Programs to find files in a file system.

## v.18. flex
A utility for generating programs that recognize patterns in text.

## v.19. gcc
The Gnu Compiler Collection.

## v.20. gdbm
The GNU Database Manager library.

## v.20. gettext-tiny
Stub and lightweight replacements of the GNU gettext suite.

## v.21. gmp
Math libraries that provide useful functions for arbitrary precision arithmetic.

## v.22. gperf
A program that generates a perfect hash function from a key set.

## v.23. grep
Programs for searching through files.

## v.24. grub
The Grand Unified Boot Loader.

## v.25. iputils
Programs for basic network administration. It's intended as a replacement for
both the unmaintained inetutils and iana-etc although it lacks many tools (the
networking stack still needs further assessment).

## v.26. intltool
Tools for extracting translatable strings from source files.

## v.27. iproute2
Programs for basic and advanced IPv4 and IPv6 networking.

## v.28. isl
A library for manipulating sets and relations of integer points bounded by
linear constraints. It's required to enable Graphite loop optimizations when
building chroot and system packages.

## v.29. kbd
Key-table files and keyboard utilities for non-US keyboards, and a number of
console fonts.

## v.30. kmod
Programs needed to administer Linux kernel modules.

## v.31. lbzip2
Parallel programs for compressing and decompressing files. It's intended as a
parallel drop-in replacement for bzip2; however, it lacks some utilities which
might be provided in the future in the form of `lbzip2-utils`.

## v.32. less
A very nice text file viewer that allows scrolling up or down when viewing a
file. It's intended as a better replacement for `more` which is disabled in the
`util-linux` ceras (package).

## v.33. libcap
Implements the user-space interfaces to the POSIX 1003.1e capabilities available
in Linux kernels. Please note that Red Hat's libcap-ng isn't a drop-in
replacement for libcap and is intended for different purposes.

## v.34. libedit
A port of the NetBSD Editline library (libedit) intended to be a drop-in
replacement for GNU readline library. This ceras (package) shouldn't be confused
for MINIX's editline.

## v.35. libffi
A portable, high level programming interface to various calling conventions.

## v.36. libressl
A version of the TLS/crypto stack forked from OpenSSL in 2014, with goals of
modernizing the codebase, improving security, and applying best practice
development processes. It's intended to be a drop-in replacement for OpenSSL.

## v.37. libstdc++-v3
The GNU Standard C++ Library v3. It's only used when building the native
toolchain, as gcc already includes it in both the final native and system
builds.

## v.38. libtool
The GNU generic library support script.

## v.39. libuargp
libuargp extracted from uclibc-ng, modified lightly and intl-friendly. It
provides argp support to musl from uclibc-ng and is intended to replace
argp-standalone which provides the same support but from GLIBC.

## v.40. linux
The Linux kernel.

## v.41. linux-headers
The Linux kernel headers.

## v.42. lz4
Extremely Fast Compression algorithm. It's used for compressing the Linux kernel
and its modules to further reduce boot times.

## v.43. m4
A general text macro processor.

## v.44. make
A program for directing the building of packages.

## v.45. mandoc
The mandoc UNIX manpage compiler toolset.

## v.46. mawk
Program for manipulating text files. It's intended to be a lighter and faster
drop-in replacement for gawk.

## v.47. meson
A software tool for automating the building of software.

## v.48. mpc
Functions for the arithmetic of complex numbers.

## v.49. mpfr
Functions for multiple precision arithmetic.

## v.50. musl
The main C library.

## v.51. musl-fts
Implementation of fts(3) for musl libc packages. This is also required to build
elfutils-libelf in order to build the Linux kernel.

## v.52. musl-obstack
A standalone library to implement GNU libc's obstack for use with musl libc.
This is also required to build elfutils-libelf in order to build the Linux
kernel.

## v.53. netbsd-curses
A port of netbsd's curses library for usage on Linux systems.

## v.54. oksh
Portable OpenBSD ksh, based on the Public Domain Korn Shell (pdksh). This is
also the main user shell.

## v.55. patch
A program for modifying or creating files by applying a patch file typically
created by the diff program.

## v.56. pcre2
A revised API for the PCRE library, which is a set of functions, written in C,
that implement regular expression pattern matching. It's needed to build some
cerata (packages) like `less` with the new version of PCRE.

## v.57. perl
An interpreter for the runtime language PERL.

## v.58. perl-xml-parser
A Perl module that interfaces with Expat.

## v.59. pigz
Parallel programs for compressing and decompressing files. It's intended as a
parallel drop-in replacement for gzip.

## v.60. pkgconf
A program which helps to configure compiler and linker flags for development
frameworks. It's intended to be a lighter drop-in replacement for pkg-config.

## v.61. procps-ng
Programs for monitoring processes.

## v.62. psmisc
Programs for displaying information about running processes.

## v.63. python
An interpreted language that has a design philosophy that emphasizes code
readability.

## v.64. rsync
An open source utility that provides fast incremental file transfer. It's used
for quickly comparing and copying source files without polluting the original
sources tree.

## v.65. s6
A small suite of programs for UNIX, designed to allow process supervision (a.k.a
service supervision), in the line of daemontools and runit, as well as various
operations on processes and daemons. 

## v.66. s6-boot-scripts
glaucus's s6 boot scripts. They still lack proper output and logging support.

## v.67. s6-linux-init
Aa set of minimalistic tools used to create a s6-based init system.

## v.68. s6-rc
A service manager for s6-based systems.

## v.69. samurai
A ninja-compatible build tool written in C99 with a focus on simplicity, speed,
and portability. It's intended to be a lighter and faster drop-in replacement
for ninja.

## v.70. sed
Allows editing of text without opening it in a text editor.

## v.71. shadow
Programs for handling passwords in a secure way.

## v.72. skalibs
A package centralizing the free software / open-source C development files
required for building s6-based systems.

## v.73. slibtool
A skinny libtool implementation, written in C. It's intended alongside sltdl to
be a drop-in replacement for libtool but it doesn't provide a libtoolize
replacement yet; hence, we're including libtool until sltdl and slibtoolize are
ready.

## v.74. texinfo
Programs for reading, writing, and converting info pages.

## v.75. toybox
All-in-one Linux command line. The custom configurations that glaucus provides
ensure that only tools that replace coreutils are built.

## v.76. util-linux
Miscellaneous utility programs.

## v.77. utmps
An implementation of the utmpx.h family of functions performing user accounting
on Unix systems because musl doesn't provide one.

## v.78. vim
An editor.

## v.79. xz
Programs for compressing and decompressing files.

## v.80. zlib-ng
Compression and decompression routines with optimizations for "next generation"
systems. It also includes a zlib compatibility mode to allow it to replace zlib.
