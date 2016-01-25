## SD mod for DIR-300 B1 with extroot pivot-root on Chaos Calmer
Manual: https://docs.google.com/document/d/1X3RId3d9MDHeSq82_6cZ_VaBjYVX7T0hU396oFHsEdA/edit

### gpiommc.c ###
File contains patched version of gpiommc.c

### openwrt-chaos-calmer-dir-300-b1-sdmod-dirryhack-factory.bin ###
OpenWRT Chaos Calmer (r48430) with DIRRY-HACK gpiommc.c

Enabled:
* kmod-gpio-over-mmc (patched)
* kmod-fs-ext4
* kmod-mmc-spi
* block-mount

Disable:
* kmod-leds-gpio
* kmos-gpio-button-hotplug
* usb support
