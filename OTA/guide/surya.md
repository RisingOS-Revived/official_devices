# RisingOS Installation Instructions for surya

**Maintainer:** [shoya0x00](https://t.me/BrainCellSG) | @shoya0x00

### Required Files

* Download the needed files from [download page](https://risingosrevived.tech/downloads.html?codename=surya)

* Required device files for first-time flash:
* recovery.img
* ...and then the latest OTA zip for surya (RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-surya-ota.zip)

*Do ***NOT*** substitute ***any*** of these files with files that you've downloaded elsewhere if you want support for your installation.*

### First time installation (clean flash):

* Prepare the device for fastboot mode:
* Power off the device.
* Press and hold **Power** + **Volume Down** buttons until Fastboot mode appears.
* Connect the device to your PC via USB cable and verify the connection with:

```
fastboot devices
```

* Flash the required images:
* recovery.img

```
fastboot flash recovery recovery.img
```

* Enter Recovery mode:
* Use the volume buttons to navigate to "Recovery Mode."
* Press the Power button to confirm.

* Perform a Factory Reset in Recovery mode
* Navigate to **"Wipe data/factory reset"**.  
* Confirm the action to clear old data.

* Install the ROM
* Use the adb sideload command with the ROM file:

``` 
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-surya-ota.zip
```

### Update installation:

* Reboot the device into Recovery mode.

* Install the update:
  * Use the adb sideload command to flash the update file:

```
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-surya-ota.zip
```

* Reboot the device:
* After installation, select **"Reboot system now"** from the Recovery menu.
 
 #### Via OTA:
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* Reboot

Your device should now be updated!