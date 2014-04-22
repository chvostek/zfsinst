## zfsinst

Install FreeBSD with root-on-ZFS.

#### Quick start:

 1. Burn the memstick image. <br/> `dd if=/path/to/FreeBSD-10.0-RELEASE-amd64-memstick.img of=/dev/da0 bs=64k`
 2. Mount the newly created image. <br/> `mount /dev/da0 /mnt`
 3. Copy the script to the image. <br/> `cp path/to/zfsinst /mnt/bin/`
 4. Unmount.
 5. Boot the memstick image.
 6. Select LiveCD.
 7. Log in as "root".
 8. Run `zfsinst`, answer the questions.
 9. PROFIT

#### To-do:

 * Provide a patch that modifies an existing memstick.img filesystem to provide `zfsinst` at the Welcome dialog as an option along-side **`<Install>`**, **`<Shell>`** and **`<Live CD>`**
 * Provide instructions for building an original memstick image (`man release` and `make memstick`)
 * Add overrides for filesystem layout (we currently assume layout based on number of raw devices)
 * Built interactivity into standard dialogs
 * Test in FreeBSD 11, modify as required

#### See also:

* https://wiki.freebsd.org/RootOnZFS

