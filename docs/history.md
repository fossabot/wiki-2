# History
glaucus initially started out as a hobby project called snail, and has thus been
under development for 2 years now.

## Aim
The aim was to create an extremely minimal Linux based operating system that
would run on modern hardware and require less than or equal to 1MB of RAM to
run.

## Experimentation
Experimentation started with the lightest possible alternatives to the current
tools used in creating cross-compilation toolchains.

The initial stage of trial and error took around 8 months. Every possible
toolchain combination with compilers ranging from `tcc`, `scc`, `pcc` and `gcc`
to binary utilities ranging from `elfutils`, `elftoolchain` and `binutils` to
standard C libraries ranging from `uClibc`, `uClibc-ng`, `dietlibc` and `musl`.

The initial goal was to test each combination, and attempt a complete build of
all suckless sbase tools followed by libressl.

A good amount of time was spent on constructing different toolchains using
various components other than GNU. The first toolchains used tcc and
elfutils/elftoolchain but failed to build a complete sbase... The second
generation of toolchains used pcc and elfutils/elftoolchain, and they were much
better, as they were able to compile all sbase tools but optimization was really
lacking, as the binaries that resulted from gcc -Os were smaller than those from
pcc -Os.

Then elfutils/elftoolchain were ditched completely as they don't work well with
musl and neither includes all utilities offered by binutils (so you'll end up
with a mixture of both trying to cover up the basic utilities offered by
binutils); hence, the choice to stick with gcc and binutils was made.

`tcc` was really fast but failed to build all suckless sbase tools and libressl
and thus failed the test. `pcc` was a close contender as it passed the test
successfully, but the resulting binaries were noticeably bigger than `gcc`'s
even at the same optimization level.

As for the binary utilities, I ditched `elftoolchain` in favor of `elfutils`
because the project wasn't as active, but then found out that `elfutils` doesn't
work well with `gcc`; hence, `binutils` was the only option left.

I didn't try LLVM as I was trying to limit the amount of cerata using c++, but I
tested libc++ once and libstdc++ was faster (due to regressions in libc++). I
didn't try lld yet, as I was interested in gold but, I went back to bfd/ld after
I knew that gold doesn't build with musl unless PIE is enabled (I didn't plan on
using PIE early on, but I'm considering it in the near future).

I might try lld in the distant future and maybe give GOLD another chance, but I
won't be changing the design of the toolchain, especially after I got it working
with the optimizations I'm using.

One year later, the goal was accomplished. snail booted successfully and ran in
under 1MB of RAM.

![snail](https://github.com/glaucuslinux/screenshots/raw/master/snail.png)

However, snail was extreme, it used an extremely minimal kernel configuration
(based on DOTSLASHLINUX kernel configuration guides) and `dash` as its sole
shell, suckless sbase and ubase for userland and sinit/svc as an init
system/service manager respectively. The root filesystem was also read-only.

## glaucus
glaucus is an attempt to fix snail and turn it into a usable distribution that's
not only extremely lightweight, but also highly optimized for performance and
much more convenient.
