# RisingOS Revived Installation Instructions for zeus

**Maintainer:** [acerhizm](https://t.me/acerhizm) | [Support group](https://t.me/acerbuilds) | [GitHub](https://github.com/acerhizmq)

**Device:** Xiaomi 12 Pro (zeus)

---

### Before you start

* Your bootloader must be unlocked.
* The ROM ships the HyperOS 3 (OS3.0.4.0) firmware, so no separate firmware flash is needed.
* Back up everything you need. A clean flash formats data, including internal storage.
* Use only the files from the download page. Do **not** mix in boot, dtbo, vendor_boot, vbmeta or recovery images from other builds or ROMs if you want support.

### Required files

Download from the [download page](https://risingosrevived.tech/downloads.html?codename=zeus):

* `RisingOS-9-xxxxxx-xxxx-GAPPS-OFFICIAL-zeus-ota.zip`
* `boot.img`, `dtbo.img`, `vendor_boot.img`, `vbmeta.img` and `recovery.img` of the **same build date** (in the `IMGs` folder)

The ROM ships with GApps, so no separate GApps package is needed.

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
fastboot flash dtbo dtbo.img
```

```
fastboot flash vendor_boot vendor_boot.img
```

```
fastboot flash vbmeta vbmeta.img
```

```
fastboot flash recovery recovery.img
```

4. Reboot to recovery:

```
fastboot reboot recovery
```

5. In recovery select **Factory reset** → **Format data / factory reset** and confirm.
6. Go back, select **Apply update** → **Apply from ADB**, then on the PC run:

```
adb sideload RisingOS-9-xxxxxx-xxxx-GAPPS-OFFICIAL-zeus-ota.zip
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
adb sideload RisingOS-9-xxxxxx-xxxx-GAPPS-OFFICIAL-zeus-ota.zip
```

3. Select **Reboot system now**.

There is no need to format data or to reflash the images when updating from an official RisingOS Revived 9.x build.

---

### Notes

* Root: KernelSU is built into the kernel. Install a KernelSU manager app to use it.
* Device settings (display, charging, audio, performance) are in **Settings → System → XiaomiParts** or the XiaomiParts app.
* When reporting a bug, include a logcat and the steps to reproduce it in the support group.

Your device should now be running RisingOS Revived!
