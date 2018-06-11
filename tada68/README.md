---
---

## Linux Flashing
```
mount -t vfat -o rw,auto,user,fmask=0000,dmask=0000,exec /dev/sdc TADA68/
```

or

```
mount -t vfat -o rw,nosuid,nodev,relatime,uid=1000,gid=1000,fmask=0022,dmask=0022,codepage=437,iocharset=iso8859-1,shortname=mixed,showexec,utf8,flush,errors=remount-ro,uhelper=udisks2 /dev/sdb TADA68/
```
