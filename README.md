# zfsinst

Install FreeBSD with root-on-ZFS.

#### Quick start:

 1. Burn the memstick image. <br/> `dd if=/path/to/FreeBSD-10.0-RELEASE-amd64-memstick.img of=/dev/da0 bs=64k`
 2. Mount the newly created image. <br/> `mount /dev/da0 /mnt`
 3. Copy the script to the image. (Yes, there is space.) <br/> `cp path/to/zfsinst /mnt/bin/`
 4. Unmount.
 5. Boot the memstick image.
 6. Select LiveCD.
 7. Log in as "root".
 8. Run `zfsinst`, answer the questions.

#### To-do:

 * Provide a patch that modifies an existing memstick.img filesystem to provide `zfsinst` as an install option at the Welcome dialog in another dialog after **`<Install>`** is selected
 * Provide instructions for building an original memstick image (n.b. `man release` and `make memstick`)
 * Add overrides for filesystem layout (we currently assume layout based on number of raw devices)
 * ~~Add option to customize name of zpool~~
 * Built interactivity into standard dialogs
 * Test in FreeBSD 11, modify as required

#### See also:

* https://wiki.freebsd.org/RootOnZFS

