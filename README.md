# For building TWRP for Xiaomi Redmi 5 Plus (Global) & Redmi Note 5 (India) ONLY

To compile:

```
. build/envsetup.sh 
lunch omni_vince-eng
mka recoveryimage
```

Kernel source: [StormBreaker-Project for vince](https://github.com/stormbreaker-project/kernel_xiaomi_vince)

## Spec Sheet

| Feature                 | Specification                     |
| :---------------------- | :-------------------------------- |
| CPU                     | Octa-core 2.0 GHz Cortex-A53      |
| Chipset                 | Qualcomm MSM8953 Snapdragon 625   |
| GPU                     | Adreno 506                        |
| Memory                  | 3/4 GB                            |
| Shipped Android Version | 7.1.2                             |
| Storage                 | 32/64 GB                          |
| MicroSD                 | Up to 256 GB                      |
| Battery                 | 4000 mAh (non-removable)          |
| Dimensions              | 151 x 76 x 8.5 mm                 |
| Display                 | 1080x2160 pixels, 5.99 (~401 PPI) |
| Rear Camera             | 12 MP, LED flash                  |
| Front Camera            | 5 MP, LED flash                   |
| Release Date            | February 2018                     |

-----------------------------------------------------------------

➜ Blocking checks
- [x] Correct screen/recovery size
- [x] Working Touch, screen
- [x] Backup to internal/microSD
- [x] Restore from internal/microSD
- [x] reboot to system
- [x] ADB

➜ Medium checks
- [x] update.zip sideload
- [x] UI colors (red/blue inversions)
- [x] Screen goes off and on
- [x] F2FS/EXT4 Support, exFAT/NTFS where supported
- [x] all important partitions listed in mount/backup lists
- [x] backup/restore to/from external (USB-OTG) storage
- [x] backup/restore to/from adb (https://gerrit.omnirom.org/#/c/15943/)
- [x] Correct date
- [x] decrypt /data

➜ Minor checks
- [x] MTP export
- [x] reboot to bootloader
- [x] reboot to recovery
- [x] poweroff
- [x] battery level
- [x] temperature
- [?] input devices via USB (USB-OTG) - keyboard, mouse(works) and disks
- [x] USB mass storage export
- [x] set brightness
- [x] vibrate
- [x] screenshot
- [x] partition SD card
- [?] encrypted backups(doesn't ask password during restore)
