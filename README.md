# frickeluschi
literate doodle debian preseed file experiement for local horror frickel hypervisor

Linkliste
---
https://www.debian.org/releases/stable/amd64/apbs03.en.html
https://gist.github.com/lorin/5140029
https://zauner.nllk.net/post/0033-debian-preseed/
https://github.com/hoedlmoser/preseed-debian/blob/main/preseed-raid-lvm.cfg
https://wiki.debian.org/tasksel#A.22standard.22_task
https://www.debian.org/blends/hamradio/get/metapackages
https://packages.debian.org/stable/
https://cockpit-project.org/applications.html
https://packages.debian.org/stable/qemu-kvm
https://secopsmonkey.com/custom-partioning-using-preseed.html

Ziele
---
bootable selfinstall usb for cockpit and ganeti equipped ´Debian Bullseye´.
[assigned <name> | written | pushed <commit> | tested]

- BOOT/EFI gap bit at 1 1 1 as /free to maintain CSM compatibility [pushed initial]
- Install Debian as an ext4 BIOS/UEFI CSM compatible OS on /dev/sda [pushed initial]
- Partition sdc/d/e as an ext4 software RAID 5 (until raidcontroller) using d-i partman mounted at /var/repo [pushed initial]
- Partition sdb as an ext4 variable storage device mounted under /var/storage [assigned Jan]
-tbc-
