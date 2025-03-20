# RisingOS Installation Instructions for topaz/tapas

**Maintainer:** @skwel24 x @mirabelle19999

---
 
## **First Installations**

## **Flashing Steps:**

• Backup your Important files

• Boot to Custom Recovery

• Format Data/Wipe Internal, Cache, Dalvik, Metadata, etc.

• Flash the **REQUIRED** Firmware **(topaz - [`2.0.9.0.VMGMIXM`](https://xmfirmwareupdater.com/archive/firmware/topaz/#) / tapas - [`2.0.9.0.VMTMIXM`](https://xmfirmwareupdater.com/archive/firmware/tapas/#))**

• Flash **RisingOS Revived** ROM

• Reflash Custom Recovery

• Reboot Recovery

• Flash **[`RO2RW`](https://t.me/CartelPH/262/2169)** (If CORE/GAPPS build: Skip this step)

• Reboot Recovery

• Flash GApps of your choice (nikGapps Recommended) (If CORE/GAPPS build: Skip this step)

• Format Data/Wipe Cache & Dalvik

• Reboot System


## **Dirty Flash Steps:**

• Boot to Custom Recovery
• Flash the **REQUIRED** Firmware **(topaz - [`2.0.9.0.VMGMIXM`](https://xmfirmwareupdater.com/archive/firmware/topaz/#) / tapas - [`2.0.9.0.VMTMIXM`](https://xmfirmwareupdater.com/archive/firmware/tapas/#))** (Optional: Skip if already flashed)

• Flash **RisingOS Revived** ROM

• Reflash Custom Recovery

• Reboot to Recovery

• Flash RO2RW (If CORE/GAPPS build: Skip this step)

• Reboot Recovery

• Flash GApps of your choice (If CORE/GAPPS build: Skip this step)

• Reboot System



### Flash via ADB Sideload:

* Enter Recovery mode:
  * Press and Hold Power Button + Volume Up button
  * Wait until it boots to Recovery

* Perform a Factory Reset in Recovery mode
* Navigate to **"Wipe data"**.  
* To confirm, type 'Yes'

* Install the ROM
* Use the adb sideload command with the ROM file:

``` 
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-VANILLA-OFFICIAL-topaz-ota.zip
```

### Update installation:

* Reboot the device into Recovery mode.

* Install the update:
  * Use the adb sideload command to flash the update file:

```
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-VANILLA-OFFICIAL-topaz-ota.zip
```

* Reboot the device:
  * After installation, select **"Reboot system now"** from the Recovery menu.
 
 #### Via OTA:
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* Reboot

Your device should now be updated!
