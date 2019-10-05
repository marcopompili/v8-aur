# V8 AUR package
V8 package for Archlinux

## Updates
### Oct-2019

* Since 7.7.299.10-1 v8 uses standard lib paths as requested (apart what is needed to run d8).
* For specific uses like R, I strongly recommend the package **v8-r** which has a custom configuration for R.

## Notes
* Latest version is based on the version on branch-heads from the V8 repositories. I stick to stable, but sometimes I could use beta, I never use dev (check this: https://omahaproxy.appspot.com/).
* This is a _"generic"_ configuration, v8 is highly configurable, if you need v8
for some specific integration please check the Google documentation.
* **Prefer yay/aurman** instead of yaourt/pacaur.
* **Gclient has to download the whole V8 repository**, it takes some time to complete (depending on your internet connection).
* This package **requires between 3 and 4 gigs of disc space** so be sure to have a large enough /tmp partition if you use yaourt, also be aware that aurman/yay/pacaur will save this package in `~/.cache/(aurman|yay|pacaur)/v8`, so be sure to have a `/home` partition with enough space.
* The build and testing process takes some time, I recommend to use at least a 4 cores with 8 threads cpu, better an 8 cores 16 threads cpu.
* If you have at least 32GB of RAM you can use a ram partition to speed up the build process (yaourt uses `/tmp` by default).
