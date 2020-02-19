# 4.5. Setting Up the Environment
Both the `.bash_profile` and `.bashrc` files should be in `/home/glaucus` when
you cloned the `glaucus` repository. So without worrying about obtaining them,
let's examine their contents.

## 4.5.1. .bash_profile
Let's start by examining the contents of the `.bash_profile` file:

```Shell
exec env -i HOME=/home/glaucus TERM=xterm-256color PS1='\u:\w$ ' /usr/bin/bash
```

The `env` commands ensures that when logged in as the `glaucus` user, a new
shell is created with an empty environment except for the `HOME`, `TERM` and
`PS1` environment variables which are set to `/home/glaucus`, `xterm-256color`
and `\u:\w$ ` respectively.

No unwanted and potentially hazardous environment variables from the host
system leak into the environment where the toolchain, the chroot environment
will be constructed. The technique used of ensuring a clean environment achieves
the goal of maximum isolation from the host system.

## 4.5.2. .bashrc
The file `.bashrc` contains the following:

```Shell
set +h
umask 022
export LC_ALL=POSIX
export PATH=/toolchain/bin:/usr/bin
unset CFLAGS CPPFLAGS CXXFLAGS LDFLAGS MAKEFLAGS
export HISTFILESIZE=
export HISTSIZE=
export HISTTIMEFORMAT='[%F %T] '
export PROMPT_COMMAND="history -a; $PROMPT_COMMAND"
```

The `set +h` command turns off `bash`'s hash function. Hashing is ordinarily a
useful feature—`bash` uses a hash table to remember the full path of executable
files to avoid searching the `PATH` time and again to find the same executable.
However, the new tools should be used as soon as they are installed. By
switching off the hash function, the shell will always search the `PATH` when a
program is to be run. As such, the shell will find the newly compiled tools in
`$TOOL` as soon as they are available without remembering a previous version of
the same program in a different location.

Setting the user file-creation mask to 022 (`umask 022`) ensures that newly
created files and directories are only writable by their owner, but are readable
and executable by anyone (assuming default modes are used by the open(2) system
call, new files will end up with permission mode 644 and directories with mode
755).

The `LC_ALL` variable controls the localization of certain programs, making
their messages follow the conventions of a specified country. Setting LC_ALL to
`POSIX` or `C` (`C` is actually an alias for `POSIX`) ensures that everything
will work as expected in the chroot environment.

By putting `/toolchain/bin` ahead of the standard `PATH`, all the programs
installed in Chapters 5 and 6 are picked up by the shell immediately after their
installation. This, combined with turning off hashing, limits the risk that old
programs are used from the host when the same programs are available in the
chapter 5 environment.

We then unset all sorts of flags (`CFLAGS`, `CPPFLAGS`, `CXXFLAGS`, `LDFLAGS`
and `MAKEFLAGS`) just to ensure that nothing leaks in from the host environment.

The rest of the export commands control `bash`'s history file, its size (we're
giving `bash` unlimited history) and formatting how the history is stored, just
to make things more convenient in case of manual intervention.
