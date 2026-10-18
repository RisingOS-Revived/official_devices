### Pre-installation:

* Make sure you have latest firmware Installed.
* Gapps package (optional)

### First time installation (clean flash):

* Flash recovery (fastboot flash recovery_ab recovery.img)
* Reboot in recovery (fastboot reboot recovery)

* In Recovery -> Apply Update -> ADB Sideload
* Install rom.zip (adb sideload RisingOS-Revived.zip)
* Reboot recovery
* Format data
* Install gapps (optional)
* Reboot system

### Update installation:
#### Via recovery (recommended way):
* Boot to recovery
* Choose rom.zip
* Reinstall gapps (if you have before)

#### Via OTA:
* Go to Settings -> System -> Software Updates -> System Updates and download latest build
* Choose install and let it finish
* If having gapps, reboot to recovery and reinstall gapps package again
* Reboot
