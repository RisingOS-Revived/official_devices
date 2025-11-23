# RisingOS Installation Instructions
## Instructions

#### First time installation (clean flash):​

## Install using Rising recovery.

* Installing a new ROM will erase all your data! Backup your data.
  
## Boot to fastboot (volume down + power button) or use this command:
***************************************************
    adb reboot bootloader
***************************************************
## Install specific device images.
***************************************************
    fastboot flash boot boot.img
    fastboot flash vendor_boot vendor_boot.img
    fastboot flash dtbo dtbo.img
***************************************************

## reboot to Rising Recovery.
***************************************************
    fastboot reboot recovery
***************************************************

## Format Data.
On the recovery screen, go to:
Factory reset, then Format data/factory reset

## Install Rom from ADB Sideload.
Go to Apply Update; then Apply Update from ADB.

On a PC:
Windows: Open a CMD or PowerShell window.

Linux/Mac: Open a window of your terminal emulator.
***************************************************
    adb sideload RisingOS_Revived-xxxxxxx.zip

*** if you have vanilla build flash GApps of your choice (Opitional)- 
***************************************************
    adb sideload gapps_filename.zip
***************************************************
Reboot to system and enjoy the new life of your Smartphone!

## Install using custom recovery

***************************************************
  * Custom recovery [Link on Rom postage]
***************************************************
Backup your data
Boot to Custom Recovery
Flash **RisingOS_Revived-Rom.zip
Format Data
*** if you have vanilla build flash GApps of your choice.
Reboot to system and enjoy the new life of your Smartphone!

#### Update installation (dirty flash):​
***************************************************
### OTA Recommended ###
Settings > System > Updater, Check for updates, download and install them, and restart when prompted.
***************************************************
## Install using Rising recovery.

Backup your data
## reboot to Rising Recovery.

## Install Rom from ADB Sideload.
Go to Apply Update; then Apply Update from ADB.

On a PC:
Windows: Open a CMD or PowerShell window.

Linux/Mac: Open a window of your terminal emulator.
***************************************************
    adb sideload RisingOS_Revived-xxxxxxx.zip

*** if you have vanilla build re-flash GApps of your choice (Opitional)- 
***************************************************
    adb sideload gapps_filename.zip

Reboot to system aand enjoy RisingOS-Revived updated with the best that a Custom Rom can offer!
***************************************************

## Install using custom recovery

***************************************************
 * Custom recovery [Link on Rom postage]
***************************************************
Backup your data
Boot to Custom Recovery
Flash **RisingOS_Revived-Rom.zip
*** if you have vanilla build flash GApps of your choice
Reboot to system and enjoy RisingOS-Revived updated with the best that a Custom Rom can offer!
