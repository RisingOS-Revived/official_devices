# RisingOS Installation Instructions for dumpling

### Required Files

- Download the following files from the [download page](https://risingosrevived.tech/downloads.html?codename=dumpling)
  - twrp-3.7.1_12-2_cheeseburger_dumpling.img or newer
  - ...and the latest OTA zip for dumpling (RisingOS_Revived-x.x-xxxxxxxx-VANILLA-OFFICIAL-dumpling-ota-signed.zip)


### First Time Installation (clean flash)

- Install the [required drivers](https://wiki.lineageos.org/adb_fastboot_guide) if not done already
- [Unlock the bootloader](https://wiki.lineageos.org/devices/dumpling/install/#unlocking-the-bootloader) if not done already
- Boot the device into fastboot mode
  - Power off the device
  - Press and hold **Power** + **Volume Down** buttons until Fastboot mode appears
  - Connect the device to your PC via USB cable and verify the connection using

```
fastboot devices
```

- Flash the recovery

```
fastboot flash recovery twrp-3.7.1_12-2_cheeseburger_dumpling.img
```

- Enter Recovery mode
  - Use the volume buttons to navigate to "Recovery Mode"
  - Press the Power button to confirm.

- Perform a Factory Reset in Recovery mode
  - Navigate to "Wipe"
  - Press Format Data and type "yes"
  - Confirm the action to clear all data

- Install the ROM

``` 
adb sideload RisingOS_Revived-x.x-xxxxxxxx-VANILLA-OFFICIAL-dumpling-ota-signed.zip
```


### Manual Update Installation

- Reboot the device into Recovery mode

- Install the update
  - Use the adb sideload command to flash the update file

```
adb sideload RisingOS_Revived-x.x-xxxxxxxx-VANILLA-OFFICIAL-dumpling-ota-signed.zip
```

- Reboot the device
  - After installation, select **"Reboot system now"** from the Recovery menu


### Via OTA

- Open the Settings App
- Navigate to System -> Updater
- Refresh the ota info with the round arrow in the top right
- Press download for the latest build (the one on top)
- Choose install and let it finish
- Reboot

Your device should now be updated
