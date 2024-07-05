/sbin contains system binaries, these commands need superuser permissions. They're used by both system administrators or the system itself.

/lib contains libraries needed by binaries.

/usr used to be what /home is now, it mirrors the structure of the root folder.

/usr/local -> again similar to root, but for 3rd-Party-Applications

/opt (optional), is used for applications that don't split their components
(e.g. IDEs or Web Browsers).

/boot -> what the system needs to start, never touch this.

/etc -> initially for anything, but emerged to be the application configuration folders.

/dev -> not development: devices. Contains drivers to interact with hardware.

/media -> this is where external storage is mounted automatically.

/mnt -> this is where we mount stuff manually.