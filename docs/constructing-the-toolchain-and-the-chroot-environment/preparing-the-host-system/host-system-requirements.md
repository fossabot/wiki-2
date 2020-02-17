# 2.2. Host System Requirements
Your host system should have the following software with the minimum versions
indicated. This should not be an issue for most modern Linux distributions. Also
note that many distributions will place software headers into separate packages,
often in the form of “<package-name>-devel” or “<package-name>-dev”. Be sure to
install those if your distribution provides them.

Earlier versions of the listed software packages may work, but have not been
tested.

*   `bash`:      5.0.11(1)-release

!!! note
    `/bin/sh` should be a symbolic or hard link to `bash`

*   `binutils`:  2.34
*   `bison`:     3.5.1

!!! note
    `/usr/bin/yacc` should be a link to bison or small script that executes
    `bison`

*   `bzip2`:     1.0.8
*   `coreutils`: 8.31
*   `diffutils`: 3.7
*   `findutils`: 4.7.0
*   `gawk`:      5.0.1

!!! note
    /usr/bin/awk should be a link to gawk

*   `gcc`:       9.2.0
*   `git`:       2.25.0
*   `glibc`:     2.31
*   `grep`:      3.4
*   `gzip`:      1.10
*   `linux`:     5.5.3-arch1-1
*   `m4`:        1.4.18
*   `make`:      4.3
*   `patch`:     2.7.6
*   `perl`:      5.30.1
*   `rsync`:     3.1.3
*   `sed`:       4.8
*   `tar`:       1.32
*   `texinfo`:   6.7
*   `xz`:        5.2.4

!!! warning
    Note that the symlinks mentioned above are required to build glaucus using
    the instructions contained within this book. Symlinks that point to other
    software (such as dash, mawk, etc.) work in the chroot environment, but
    haven't been tested on the host system yet.

To see whether your host system has all the appropriate versions, and the
ability to compile programs, run the following (after having cloned the glaucus
repository):

```Shell
dash /home/glaucus/scripts/require
```

You should get an output in the following format:

```Shell
bash:      5.0.11(1)-release
binutils:  2.34
bison:     3.5.1
bzip2:     1.0.8
coreutils: 8.31
diffutils: 3.7
findutils: 4.7.0
gawk:      5.0.1
gcc:       9.2.0
git:       2.25.0
glibc:     2.31
grep:      3.4
gzip:      1.10
linux:     5.5.3-arch1-1
m4:        1.4.18
make:      4.3
patch:     2.7.6
perl:      5.30.1
rsync:     3.1.3
sed:       4.8
tar:       1.32
texinfo:   6.7
xz:        5.2.4
```
