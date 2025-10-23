![Installation Guide For RisingOS Revived](https://github.com/RisingOS-OSS/android/blob/fifteen/risingOS_banner.png)

### Installation Guide For RisingOS Revived on Realme 7/Narzo 20 Pro/Narzo 30 4G - salaa
 
> [!Warning]
> * Your warranty is void. Or valid, probably?
> * RisingOS Revived is not responsible for any damage you made to your device. You have been warned!
> * We are not responsible for anything that may happen to your phone by installing custom ROMs.
> * We are not responsible for anything that may happen to your phone by installing any kernels.
> * You do it at your own risk and take the responsibility upon yourself
> * You are not to blame RisingOS Revived or its respected developers for any of your loss.
>
> **Basic Notes for all users:**  
> * The provided instructions are for RisingOS Revived based on Android 15.
> * These will only work if you follow every section and step precisely
> * Do not continue after something fails! Contact in support group for help
> * The device must have an unlocked bootloader & has Platform Tools installed in pc.
> * If you are moving from any other Android version to Android 15, it is necessary to do CLEAN FLASH (Format Data)
> * Take a backup for safe side (If you are coming from older Android version or doing a clean flash)
> * For any queries or help related to Rising, join our support group : [Tap Here](https://t.me/RisingOSRevived)
> * 

### Step 1: Download Required Files
1. Download the latest Android platform tools for Windows from the link below:
   - **Platform Tools Link (Windows)**: [platform-tools-latest-windows.zip](https://dl.google.com/android/repository/platform-tools-latest-windows.zip)

2. Download the Recovery from the link below:
   - **Recovery Link [ For Android 15 ]:** [Recovery](https://t.me/FilesArchieve/251).
   
3. Download the RisingOS Revived ROM for Realme 7/Narzo 20 Pro/Narzo 30 4G - salaa from a reliable source.
   - **RisingOS Revived ROM Link**: [DOWNLOAD](https://risingosrevived.tech/device/salaa)

4. Download the firmware from the link below:
   - **Realme UI 3.0 Firmware Link**: [DOWNLOAD](https://t.me/FilesArchieve/242)

### Step 2: Bootloader Unlock: RealmeUI 3.0: (For first time users ONLY)
1. Download [Deeptest_rui3.0.apk](https://t.me/realme_7_cloud/50) install it.
2. Open apk and apply for In-depth testing then close DeepTesting app from Recent apps.
3. Turn On OEM Unlock & USB Debugging toggle from Devloper Option.
3. After 5 Minutes open DeepTesting app. Click on Query Approval Status from right corner. Tap on Start deep testing. It will boot into bootloader mode.
4. Connect your device from Pc, (MTK AND PLATFORM TOOL MUST BE INSTALLED ON SYSTEM) and pass command via cmd:
```
fastboot flashing unlock
```

5. After it's will ask you to press Volume Up and Down Press Conformation Button Corresponding To Yes. after it type:
```
fastboot reboot
```

6. Device will be Cleaned and reboot.

### Step 3: Install ADB and Boot into Fastboot Mode
1. Make sure you have ADB (Android Debug Bridge) installed on your computer. 
2. Extract the downloaded platform-tools zip file on your computer.
3. Connect your device to your computer using a USB cable.
4. Open a command prompt (Windows) or terminal (macOS and Linux) on your computer.
5. Navigate to the location where you extracted the platform-tools.
6. Enter the following command to check if your device is connected and detected by ADB:
```
adb devices
```

> [!Important]
> If your device is listed, proceed to the next step. If not, make sure your device is connected properly and that USB debugging is enabled in the developer options.

7. Now, reboot your device into Fastboot Mode using the following command:
```
adb reboot bootloader
```

### Step 4: Flash Recovery using Fastboot
1. Once your device is in Fastboot Mode, use the following command to check if Fastboot still detects your device:
```
fastboot devices
```

If your device is listed, you are ready to flash the Recovery.

2. Download the Recovery in Step 1.

3. Place the downloaded Recovery (`.img` file) in the same location as the platform-tools folder on your computer.

4. Now, flash the Recovery using the following command:
```
fastboot flash recovery recovery_file_name.img
```

> [!Important]
> Replace `recovery_file_name.img` with the actual name of the Recovery image you downloaded if needed.

5. After flashing the recovery, use the following command to reboot your Recovery:
```
fastboot reboot recovery
```

Your device will reboot with Recovery installed.

### Step 5: Wipe Data
1. In Recovery, use the touch screen or physical buttons to navigate.

2. Select "Wipe" from the main menu.

3. Format data. And reboot to recovery again.

### Step 6: Flash RisingOS Revived ROM
- Method To Flash Rom From RUI2!
1. Reboot recovery on (RUI2)
2. Flash firmware script - PROVIDED IN STEP 1
3. Flash recovery - LINK PROVIDED IN STEP 1
4. Reboot recovery
5. Format data
6. Flash ROM ( adb sideload <drag and drop ROM.zip )
7. Flash Gapps & Magisk [optional]
8. Format Data & Reboot

- Method to Flash Rom From RUI3!
1. Copy the RisingOS Revived ROM file to Internal storage or use OTG/SD card
2. In the main menu in recovery.
3. Navigate to File manager
4. Navigate to the location where you downloaded the RisingOS Revived ROM.
5. Flash ROM ( adb sideload <drag and drop ROM.zip>)
6. After insatlling successfully reboot to system.

### Clean Flash
```
- Download the latest build
- Take a backup for safe side
- Boot to Recovery - use A15 recovery - LINK PROVIDED IN STEP 1
- Format Data
- Flash the latest build
- Clear Dalvik & Cache
- Reboot to System
```

### Dirty Flash
```
1. Download the Latest Build
2. Boot to A15 recovery (eg. Ofox)
3. Flash ROM zip
4. Clear Dalvik and Cache in advance wipe
5. Reboot to System
```
- For OTA updates use [Recovery](https://t.me/FilesArchieve/251)

> [!Note] 
> **Notes specific to device build**
> - Please note that the first boot may take some time, so be patient. Once the device boots up, follow the on-screen setup instructions, and you should be ready to explore the new ROM.**
> - Remember, flashing custom ROMs carries some risks, and it may void your warranty. Make sure you understand the process and its consequences before proceeding.
> - Enjoy your new RisingOS Revived ROM experience on salaa!

<br>

> @EvilAnsh