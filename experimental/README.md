### Overview

**This is an experimental folder with just basic stuff to get everyone going.**

To get started
  - create a folder with your binary files, currently scripts expect 'android/master',
  - to this folder copy or link the following files:
    - android_system_disk_syslinux.img
    - kernel
    - gce_ramdisk.img
    - ramdisk.img
    - system.img
    - userdata.img

Use the 'start' script as a super-user. This tool will configure bridge and
start qemu for you in a screen:

    sudo ./start

### Useful info:

  - Metadata attributes sit in `etc/avd/metadata.json` file.
  - Your AVD will be assigned an IP in range 192.168.99.10 - 192.168.99.13.
  - Network interface to QEMU will be named 'android0'. Bridge is 'abr0'.
  - Metadata is served from 192.168.99.1, port 16925 (notice subtle
    difference!).

Good luck, have fun!
ender