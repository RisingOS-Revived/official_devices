# RisingOS Installation Instructions for vermeer

**Maintainer:** [Lunark :3](https://t.me/PocoF6ProSupport) | @ByteWave1014

# Preparation
* Flash the Firmware OS2.0.102.0.VNKMIXM

### Required Recovery

* Download the needed recovery from [download page](https://sourceforge.net/projects/risingos-revived/files/7.x/GAPPS/vermeer/IMGs/recovery.img/download)

* Required device recovery for first-time flash:
  * recovery.img
  * ...and then the latest OTA zip for vermeer (RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-vermeer-ota.zip)

### First time installation (clean flash):
* Prepare the device for fastboot mode:
* Power off the device.
* Press and hold **Power** + **Volume Down** buttons until Fastboot mode appears.
* Connect the device to your PC via USB cable and verify the connection with:

```
fastboot devices
```
* Flash the required recovery:
* recovery.img

```
fastboot flash recovery_ab recovery.img
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
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-vermeer-ota.zip
```

* In case you want to follow the guide in more detail check my guide in XDA [XDA](https://xdaforums.com/t/guide-to-installing-aosp-roms-for-vermeer.4720204/)

### Update installation:
 
* Reboot the device into Recovery mode.
 
* Install the update:
  * Use the adb sideload command to flash the update file:
 
```
adb sideload RisingOS_Revived-x.x.x-xxxxxxxx-GAPPS-OFFICIAL-vermeer-ota.zip
```
 
* Reboot the device:
  * After installation, select **"Reboot system now"** from the Recovery menu.

#### Via OTA:
* Go to Settings -> System -> Updater and download latest build
* Choose install and let it finish
* Reboot
 
Your device should now be updated!
