# 6.25. Stripping
It is generally considered beneficial to learn that unnecessary items can be
removed. The executables and libraries built so far contain about ??? MB of
unneeded debugging symbols that are removed automatically by the
`/home/glaucus/scripts/chroot/clean` script.

Let's look at what this script contains:

```Shell
...
find $TOOL -name *.la -delete &&

strip -gv $TOOL/lib/* &&
/usr/bin/strip --strip-unneeded -v $TOOL/bin/* &&

rm -frv $TOOL/share/doc $TOOL/share/info $TOOL/share/man
```
