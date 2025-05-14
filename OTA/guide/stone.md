# RisingOS Installation Instructions
## Instructions

#### First time installation (clean flash):​

## Install using Rising recovery.

Backup your data
Boot to fastboot and flash recovery (volume down + power button)
fastboot flash boot boot.img
Boot to Rising recovery (volume up + power button)
Format Data
adb sideload RisingOS_Revived-xxxxxxx.zip
*** if you have vanilla build flash GApps of your choice - adb sideload gapps_filename.zip
Reboot to system

## Install using custom recovery

​Backup your data
Boot to Custom Recovery
Flash **RisingOS_Revived-xxxxx.zip
Format Data
*** if you have vanilla build flash GApps of your choice


#### Update installation (dirty flash):​

## Install using Rising recovery.

Backup your data
Boot to Evolution-X recovery (volume up + power button)
adb sideload EvolutionX-15.0-xxxxxxx.zip
Reboot to system

## Install using custom recovery

​Backup your data
Boot to Custom Recovery
Flash **RisingOS_Revived-xxxxx.zip
*** if you have vanilla build flash GApps of your choice

