# 4.2. Adding the glaucus User and Group
Run the following commands as root (you can skip the first command if
`/etc/login.def` contains `USERGROUPS_ENAB yes` which is the default behaviour): 

```Shell
groupadd glaucus
useradd -g glaucus -k /dev/null -ms /bin/bash glaucus
```

Now, also as root, give the newly created `glaucus` user a password and confirm
it:

```Shell
passwd glaucus
```

Next login as `glaucus`:

```Shell
su - glaucus
```

In order for the `.bash_profile` and `.bashrc` files to take effect, you need to
first logout:

```Shell
exit
```

Then log back in:

```Shell
su - glaucus
```
