## Layout Editor

You can use the official QMK layout editor for tada68 [here](https://config.qmk.fm/#/tada68/LAYOUT_ansi)

## Flashing on Linux

If the "TADA68" USB mass storage device is not mounted automatically 
after a few seconds 
you'll have to manually mount the mass storage device.
Try running the following commands where "/dev/sdX" is the device path
that shows up after entering the reset mode.

```
mount -t vfat -o rw,auto,user,fmask=0000,dmask=0000,exec /dev/sdX /mnt/TADA68/
```

or

```
mount -t vfat -o rw,nosuid,nodev,relatime,uid=1000,gid=1000,fmask=0022,dmask=0022,codepage=437,iocharset=iso8859-1,shortname=mixed,showexec,utf8,flush,errors=remount-ro,uhelper=udisks2 /dev/sdX /mnt/TADA68/
```
