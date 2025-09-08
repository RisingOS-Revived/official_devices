# RisingOS Installation Instructions for taoyao

**Maintainer:** [ammarbahtiarasli](https://t.me/taoyao-aosp) | @ammarbahtiarasli

### Required Files

* Download the needed files from [download page](https://risingosrevived.tech/downloads.html?codename=taoyao)

* Required device files for first-time flash:
  * boot.img
  * dtbo.img
  * vendor_boot.img
  * ...and then the latest OTA zip for taoyao (RisingOS_Revived-x.x.x-xxxxxxxx-CORE-OFFICIAL-taoyao-ota.zip)

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
* boot.img
* dtbo.img
* vendor_boot.img

```
fastboot flash boot boot.img
```

```
fastboot flash dtbo dtbo.img
```

```
fastboot flash vendor_boot vendor_boot.img
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
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-CORE-OFFICIAL-taoyao-ota.zip
```

### Update installation:

* Reboot the device into Recovery mode.

* Install the update:
  * Use the adb sideload command to flash the update file:

```
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-CORE-OFFICIAL-taoyao-ota.zip
```

* Reboot the device:
  * After installation, select **"Reboot system now"** from the Recovery menu.
 
 #### Via OTA:
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* Reboot

Your device should now be updated!