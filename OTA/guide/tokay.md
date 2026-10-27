# RisingOS Revived Installation Instructions for Google Pixel 9 (tokay)

**Maintainer:** [vilckindima](https://t.me/Dimoncofe)

## Before you start

- The bootloader must be unlocked.
- Update the phone to the latest stock Android 17 firmware first: these builds need at least the October 2026 firmware (CP3A.261005.005). The ROM does not update the bootloader or the modem.
- Download the files of the same build from SourceForge (risingos-revived → 9.x → GAPPS → tokay):
  - `RisingOS-9-<date>-GAPPS-OFFICIAL-tokay-ota.zip`
  - from the `IMGs` folder: `<date>-boot.img`, `<date>-dtbo.img`, `<date>-vendor_boot.img` and `<date>-vendor_kernel_boot.img`, with the same `<date>` as in the zip name
- Back up your data: a clean flash erases everything on the phone.

## Clean flash (from stock or another ROM)

1. Reboot to the bootloader: `adb reboot bootloader`, or hold Power + Volume Down while the phone is off.
2. Flash the images:
   ```
   fastboot flash boot <date>-boot.img
   fastboot flash dtbo <date>-dtbo.img
   fastboot flash vendor_boot <date>-vendor_boot.img
   fastboot flash vendor_kernel_boot <date>-vendor_kernel_boot.img
   ```
3. Reboot to recovery: `fastboot reboot recovery`.
4. Choose **Factory reset → Format data/factory reset** and confirm.
5. Choose **Apply update → Apply from ADB**, then on the computer run:
   ```
   adb sideload RisingOS-9-<date>-GAPPS-OFFICIAL-tokay-ota.zip
   ```
6. Choose **Reboot system now**. The first boot takes a few minutes.

## Updates

- **OTA:** Settings → System → System updates, download and install the update, then reboot.
- **Manually:** reboot to recovery, choose **Apply update → Apply from ADB**, run `adb sideload` with the new zip and reboot. The images are not needed for updates.
