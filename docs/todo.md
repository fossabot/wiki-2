# TODO
1. Replace musl malloc with Jemalloc (always without relying on environment
   variable)

2. Fix jemalloc segfault (at ip)

3. Disable/Enable stuff that are auto detected

4. Create a bootable image capable of building itself from source

5. Apply K&R (tabs = 2 spaces) shell syntax styles

6. Check licenses and dependencies

7. Switch back to -march=x86-64 for release of cerata on github

8. Fill in the README files for all cerata

9. Give approximate time needed to compile each package based on my CPU

12. Add conflicts to radula

13. Add dependency resolution using tsort to radula

14. Create a variables file for building Xorg.... to get all packages reading
    its variables

15. Fix graphics and start SwayWM

16. Remove -e from single expression seds

17. Disable Libdatrie and libthai support from pango and see if it works

18. Harden the toolchain and executables (SSP and PIE)

19. gcompat for running glibc executables on musl
