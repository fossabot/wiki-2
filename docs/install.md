# Install (Outdated)
## 0. Create the `glaucus` user and group
Run the following commands as root (you can skip the first command if
`/etc/login.def` contains `USERGROUPS_ENAB yes` which is the default behaviour):
```shell
groupadd glaucus
useradd -g glaucus -k /dev/null -ms /bin/bash glaucus
```

Now, also as root, give the newly created `glaucus` user a password and confirm
it:
```shell
passwd glaucus
```

Next login as `glaucus`:
```shell
su - glaucus
```

## 1. Clone the `glaucus` repository
Make sure that you're in glaucus's user home directory `/home/glaucus` as that's
where glaucus will be built:
```shell
cd /home/glaucus
```

Pick any of the following mirrors:
* [GitHub](https://github.com/glaucuslinux/glaucus)
* [GitLab](https://gitlab.com/glaucuslinux/glaucus)
* [NotABug](https://notabug.org/glaucuslinux/glaucus)
* [BitBucket](https://bitbucket.org/glaucuslinux/glaucus)
* [Framagit](https://framagit.org/glaucuslinux/glaucus)
* [SourceForge](https://git.code.sf.net/p/glaucuslinux/glaucus)

And clone it into your existing (currently empty) working directory
`/home/glaucus`:
```shell
git clone https://github.com/glaucuslinux/glaucus .
```

## 2. Logout and log back in
In order for the `.bash_profile` and `.bashrc` files to take effect, you need to
first logout:
```shell
exit
```

Then log back in:
```shell
su - glaucus
```

## 3. Initialize the `glaucus` repository
Before you can commence constructing glaucus, you need to initialize the
`glaucus` repository that you've cloned in order to populate it with required
directories:
```shell
cd /home/glaucus
dash /home/glaucus/scripts/initialize.sh
```

## 4. Constructing the toolchain
```shell
cd /home/glaucus
time dash /home/glaucus/scripts/toolchain/run.sh
```

## 5. Constructing the chroot environment
```shell
cd /home/glaucus
time dash /home/glaucus/scripts/chroot/run.sh
```

## 6. Construct and envenomate the final system
```shell
cd /
time dash /scripts/system/run.sh
```

## 7. Logout
```shell
exit
```

## 8. Create a bootable image
```shell
cd /home/glaucus
time dash /home/glaucus/scripts/system/img.sh
```
