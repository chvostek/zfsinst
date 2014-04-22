## zfsinst

Install FreeBSD with root-on-ZFS.

### Quick start:

1 Burn the memstick image. <br/> `dd if=/path/to/FreeBSD-10.0-RELEASE-amd64-memstick.img of=/dev/da0 bs=64k`
1 Mount the newly created image. <br/> `mount /dev/da0 /mnt`
1 Copy the script to the image. <br/> `cp path/to/zfsinst /mnt/bin/`
1 Unmount.
1 Boot the memstick image.
1 Select LiveCD.
1 Log in as "root".
1 run `zfsinst`

### See also:

* https://wiki.freebsd.org/RootOnZFS

