# QEMU (Outdated)
Although glaucus is intended to be run natively on any `x86-64` machine, it's
still in under heavy development and only runs under QEMU for now.

The commands here are only to get the img files up and running (meaning that it
still needs more research on how to get the best performance with QEMU, while
staying extremely lightweight. Relevant QEMU flags also need to be
investigated).

## Binary glaucus If you've already downloaded one of (currently) two provided
glaucus img files, then all you need to do is:

1. login as your normal regular user (you know the one you're using to login
   your display manager or login manager, the one that has access to X, DISPLAY,
   GUI...)

2. Make sure `qemu` is installed and run the following:
  * if you've downloaded the glaucus core:

```shell
qemu-system-x86_64 \
  -enable-kvm \
  -hda glaucus-core-x86_64-31082019.img
```

  * Or the following if you've downloaded glaucus extra:

```shell
qemu-system-x86_64 \
  -enable-kvm \
  -hda glaucus-extra-x86_64-01092019.img
```

3. Type in `root` as the user and leave the password empty and press `enter` and
you should be in!

## Source glaucus
After having built glaucus with `-march=native` in `scripts/Variables` run the
following:

1. Login as your normal regular user (you know the one you're using to login
your display manager or login manager, the one that has access to X, DISPLAY,
GUI...)

2. Run the following (don't forget to add `-cpu host` or you'll get a kernel
panic):
```shell
qemu-system-x86_64 \
  -enable-kvm \
  -cpu host \
  -hda glaucus.img
```

## TODO
* Leverage the use of QXL
* Improve virtualization with QEMU
