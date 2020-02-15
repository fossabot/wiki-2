# vii. Typography
This section includes the typographical conventions used in this book.

## vii.1. Code Blocks
Most of the code blocks in this book will be in the form of a shell function
that either belongs to the cross or native toolchains, the chroot environment or
the system cerata (packages):

```Shell
prepare_cross() {
  install -dv $XBLD/$nom &&
  cd $XBLD/$nom
}
```

Logical lines that end with a backslash `\` are extended to two or more physical
lines.

```Shell
configure_cross() {
  $SRCD/$nom/$nom-$ver/configure \
    --prefix=$TOOL \
    --target=$TUPL \
    --enable-deterministic-archives \
    --disable-compressed-debug-sections \
    --disable-werror \
    --disable-nls \
    --with-lib-path=$TOOL/lib \
    --with-sysroot=$GLAD \
    --disable-multilib
}
```

You may also see small code blocks in the form of single words or one-line
commands or paths. For example a small code block is always used when talking
about a cerata (e.g. `binutils`).

## vii.2. Error Reporting
The `&&` at the end of the line, is used to abort the script when any command
fails (exits with a non-zero exit status).

When a command fails the running script will automatically abort and return the
exit status of the failing function along with the ceras (package) it failed at
and at what function (prepare, configure, build or install) and in which stage
(cross, native, chroot and system). This will be displayed in the following
format:

!!! failure
    $stage $ceras $function exited with status $?

## vii.3. Notes
If a certain section requires additional information that should be known but
isn't directly included or explained in the section, or if the section is
subject to change or has room for further improvement then notes in the
following format will be displayed:

!!! note
    GNU's gold linker doesn't like musl, as it refuses to build without
    enabling PIE support, and bloats things up after enabling PIE support
    and yet manages to still fail:

    <https://github.com/NixOS/nixpkgs/issues/49071>

## vii.4. Warnings
When a warning is shown you should pay attention to what it says as it'll likely
asking for escalated permissions or it denotes that a command could alter your
main host system in some way.

Here's how warnings are displayed:

!!! warning
    Be careful as the CPPFLAGS environment variable isn't honored, but the
    CFLAGS environment variable is!

## vii.5. Bugs
If there's a bug with a certain version of any used cerata (package) then it'll
be displayed in the following format:

!!! bug
    procps-ng 3.3.15 doesn't like gettext-tiny's autopoint that much:

    <https://github.com/sabotage-linux/gettext-tiny/issues/25>
