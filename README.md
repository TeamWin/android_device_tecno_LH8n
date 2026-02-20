# twrp device tree for Tecno Pova 5 pro ( LH8n )

Tecno Pova 5 Pro ( _LH8n_ ) is a mid-range smartphone from Tecno

Released on 2023, August 01

# Device SPecifications
Basic   | Spec Sheet
-------:|:-------------------------
CPU     | Octa-core (2x2.4 GHz Cortex-A76 & 6x2.0 GHz Cortex-A55)
Chipset | MediaTek Dimensity 6080 (MT6833)
GPU     | Mali-G57 MC2
Memory  | 8 GB RAM
Shipped Android Version | 13 (HIOS 13.1) ~ upgradable to hios 14 ~
Storage | 128/256 GB (UFS)
Battery | 5000 mAh, non-removable
Display | 1080 x 2460 pixels,6.78 inches, 60/90/120hz

# picture
![poba5pro](https://github.com/user-attachments/assets/0bfd51aa-7b85-4d65-afe7-602bfc4cb12e)

# Checks
Blocking checks
- [✔] Correct screen/recovery size
- [✔] Working Touch, screen
- [✔] Backup to internal/microSD
- [✔] Restore from internal/microSD
- [✔] reboot to system
- [✔] ADB

Medium checks
- [✔] update.zip sideload
- [✔] UI colors (red/blue inversions)
- [✔] Screen goes off and on
- [✔] F2FS/EXT4 Support, exFAT/NTFS where supported
- [✔] all important partitions listed in mount/backup lists
- [✔] backup/restore to/from external (USB-OTG) storage
- [?] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [✔] decrypt /data
- [✔] Correct date

Minor checks
- [✔] MTP export
- [✔] reboot to bootloader
- [✔] reboot to recovery
- [✔] poweroff
- [✔] battery level
- [✔] temperature
- [?] encrypted backups
- [✔] encrypted backups
- [✔] input devices via USB (USB-OTG) - keyboard and mouse
- [✔] USB mass storage export
- [✔] set brightness
- [✔] vibrate
- [✔] screenshot
- [✔] partition SD card
- [✔] Fastbootd

# Clone
    git clone https://github.com/naden01/tecno_LH8n.git -b android-12.1 device/tecno/LH8n

# Build
    export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch twrp_LH8n-eng; mka vendorbootimage

# Reference
- [ramabondanp ](https://github.com/ramabondanp) - Common Tree
- [Shivelight](https://github.com/Shivelight) - Touch Fix 