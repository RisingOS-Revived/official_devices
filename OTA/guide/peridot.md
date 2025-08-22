# RisingOS Installation steps for peridot

**Maintainers:**

[Farrukh Seyer Hasan](https://t.me/peridotxkernel/15833) | @Farrukh2002 | [Atharva Swamy](https://t.me/peridotsg) | @ath1188
### Required Files

* Download the needed files from [SourceForge](https://sourceforge.net/projects/risingos-revived/files/8.x/GAPPS/peridot/)

* Required device files for first-time flash:
  * boot.img
  * recovery.img
  * ...and then the latest OTA zip for peridot (RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-peridot-ota.zip)

### First time installation (clean flash):

* Make sure you are on a HyperOS 2 based ROM.
* Prepare the device for fastboot mode:
* Power off the device.
* Press and hold **Power** + **Volume Down** buttons until Fastboot mode appears.
* Connect the device to your PC via USB cable and verify the connection with:
  * ```fastboot devices```

* Flash the required images:
* boot.img
  * ``` fastboot flash boot boot.img```
* recovery.img
  * ```fastboot flash recovery recovery.img```

* Enter Recovery mode:
  * Use the fastboot command to go to recovery mode.
    * ```fastboot reboot recovery```

* Perform a Factory Reset in Recovery mode
* Navigate to **"Wipe data/factory reset"**.
* Confirm the action to clear old data.

* Install the ROM
  * Use the adb sideload command with the ROM file:
    * ```adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-peridot-ota.zip```

### Update installation:

* Reboot the device into Recovery mode.

* Install the update:
  * Use the adb sideload command to flash the update file:
    * ```adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-peridot-ota.zip```

* Reboot the device:
  * After installation, select **"Reboot system now"** from the Recovery menu.
 
 #### Via OTA:
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* Reboot

Your device should now be updated!
