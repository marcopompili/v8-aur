# V8 AUR package
V8 package for Archlinux

## Some notes

* Prefer yay/aurman instead of yaourt/pacaur.
* Gclient has to download the whole V8 repo, it takes some time to complete (depending on your internet connection).
* This package requires around 3/4 gigs of space so be sure to have a large enough /tmp partition if you use yaourt, also be aware that aurman/yay/pacaur will save this package in ~/.cache/(aurman|yay|pacaur)/v8, so be sure to have a /home partition with enough space.
* The build and testing process takes some time, I recommend to use at least a 4 cores with 8 threads CPU, better an 8 cores 16 threads CPU.
* If you have at least 32GB of RAM you can use a ram partition to speed up the build process (yaourt uses /tmp by default).
