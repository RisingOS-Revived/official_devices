# RisingOS Installation Instructions

**Author:** answer35

-------------------------------

## **Instructions**

### **ALWAYS Keep in Mind...**

> **Note:** Clean flash involves formatting data, which means you will lose data stored in the internal storage of your device. Data in the SD card should not be affected. I will not be responsible for any loss of data.

## When do a clean flash? Here you go...**
- You are coming from any other ROM.
- You are coming from a previous Android version.
- If you face issues like poor RAM management or storage problems, it indicates that you have not followed the instructions or have changed the kernel/recovery. STRICTLY follow the provided instructions before reporting any issues.

-------------------------------
 
### **Installation Methods**

### Required Files

- Download the following files from the [download page](https://risingosrevived.tech/downloads.html?codename=instantnoodlep)
  * recovery.img
  * boot.img
  * dtbo.img
  * vbmeta.img
  * ...and then the latest OTA zip for instantnoodlep from the [edition](https://sourceforge.net/projects/risingos-revived/files/7.x/) you need

### First Time Installation (clean flash)

- Install the [required drivers](https://wiki.lineageos.org/adb_fastboot_guide) if not done already
- [Unlock the bootloader](https://wiki.lineageos.org/devices/instantnoodlep/install/#unlocking-the-bootloader) if not done already. Make sure to have backed up your data before unlocking bootloader since it will erase all data on your device.
- Boot the device into fastboot mode
  - Power off the device
  - Press and hold **Power** + **Volume Down** buttons until Fastboot mode appears
  - Connect the device to your PC via USB cable and verify the connection using

```
fastboot devices
```
- Flash the required files

```
fastboot flash boot boot.img

fastboot flash dtbo dtbo.img

fastboot flash vbmeta vbmeta.img
```

- Flash the recovery

```
fastboot flash recovery recovery.img
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
adb sideload RisingOS_Revived-x.x-xxxxxxxx-xxxx-OFFICIAL-instantnoodlep-ota.zip
```

### Manual Update Installation

- Reboot the device into Recovery mode

- Install the update
  - Use the adb sideload command to flash the update file

```
adb sideload RisingOS_Revived-x.x-xxxxxxxx-xxxx-OFFICIAL-instantnoodlep-ota.zip
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
