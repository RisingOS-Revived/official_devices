# RisingOS Revived Installation Instructions for veux

**Maintainer:** [acerhizm](https://t.me/acerhizm) | [Support group](https://t.me/acerbuilds) | [GitHub](https://github.com/acerhizmq)

**Device:** Redmi Note 11 Pro 5G / Redmi Note 11E Pro / POCO X4 Pro 5G (veux)

---

### Before you start

* Your bootloader must be unlocked.
* Be on the latest stock firmware for your device before flashing for the first time.
* Back up everything you need. A clean flash formats data, including internal storage.
* Use only the files from the download page. Do **not** mix in boot, vendor_boot or vbmeta images from other builds or ROMs if you want support.

### Required files

Download from the [download page](https://risingosrevived.tech/downloads.html?codename=veux):

* `RisingOS-9-xxxxxx-xxxx-GAPPS-OFFICIAL-veux-ota.zip`
* `boot.img`, `vendor_boot.img` and `vbmeta.img` of the **same build date** (in the `IMGs` folder)

The ROM ships with GApps, so no separate GApps package is needed. Recovery is part of `vendor_boot.img`.

---

### Clean flash (first install, coming from another ROM or from Android 16)

1. Power off the phone, then hold **Power + Volume Down** to enter Fastboot mode and connect it to your PC.
2. Check the connection:

```
fastboot devices
```

3. Flash the images:

```
fastboot flash boot boot.img
```

```
fastboot flash vendor_boot vendor_boot.img
```

```
fastboot flash vbmeta vbmeta.img
```

4. Reboot to recovery:

```
fastboot reboot recovery
```

5. In recovery select **Factory reset** → **Format data / factory reset** and confirm.
6. Go back, select **Apply update** → **Apply from ADB**, then on the PC run:

```
adb sideload RisingOS-9-xxxxxx-xxxx-GAPPS-OFFICIAL-veux-ota.zip
```

7. When the sideload finishes, select **Reboot system now**. The first boot takes a few minutes.

---

### Update (dirty flash)

#### Via OTA (recommended)

* Go to **Settings → System → Updater**, download the latest build, install it and reboot.

#### Manually

1. Reboot to recovery.
2. Select **Apply update** → **Apply from ADB** and run:

```
adb sideload RisingOS-9-xxxxxx-xxxx-GAPPS-OFFICIAL-veux-ota.zip
```

3. Select **Reboot system now**.

There is no need to format data or to reflash the images when updating from an official RisingOS Revived 9.x build.

---

### Notes

* Root: KernelSU is built into the kernel. Install a KernelSU manager app to use it.
* Device settings (display, charging, audio, performance) are in **Settings → System → XiaomiParts** or the XiaomiParts app.
* When reporting a bug, include a logcat and the steps to reproduce it in the support group.

Your device should now be running RisingOS Revived!
