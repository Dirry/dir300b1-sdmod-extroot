## SD mod for DIR-300 B1 with extroot pivot-root on Chaos Calmer
Manual: https://docs.google.com/document/d/1X3RId3d9MDHeSq82_6cZ_VaBjYVX7T0hU396oFHsEdA/edit

### openwrt-chaos-calmer-rt305x-dir-300-b1-squashfs-factory-dirryhack.bin

OpenWRT Chaos Calmer factory image with DIRRY SD card hack gpiommc.

Packages:
* kmod-gpio-over-mmc (patched)
* kmod-fs-ext4
* block-mount
* fdisk
* e2fsprogs (mkfs.ext2, mkfs.ext3, mkfs.ext4)