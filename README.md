## SD mod for DIR-300 B1 with extroot pivot-root on Chaos Calmer
Manual: https://docs.google.com/document/d/1X3RId3d9MDHeSq82_6cZ_VaBjYVX7T0hU396oFHsEdA/edit

### bin-files

OpenWRT Chaos Calmer images with DIRRY SD card hack gpiommc.

Packages:
* kmod-gpio-over-mmc (patched)
* kmod-fs-ext4

### Update gpiommc.c with DIRRY HACK patch

done with: diff -Naur ./original/gpiommc.c ./modified/gpiommc.c > 865-gpiommc_dirry_hack.patch

and then modified --- and +++ first two lines as in this patch:

./chaos_calmer/target/linux/generic/patches-3.18/864-gpiommc_configfs_locking.patch

cp openwrtsetup/865-gpiommc_dirry_hack.patch ./chaos_calmer/target/linux/generic/patches-3.18/

Then compile.
