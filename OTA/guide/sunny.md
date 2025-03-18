# RisingOS Installation Instructions

**Author:** dpenra

---



## **Instructions**

### **Keep in Mind...**

- **DO NOT** try to change the included kernel.
- The system is **Read-Only** (restricts changes to overlays, system APKs, etc.).
- **DO NOT USE** any recovery other than RisingOS Recovery, which is included.
- You **MUST** format data with the provided RisingOS Recovery.

### **You MUST Clean Flash If:**

- You are coming from any other ROM or MIUI.
- You are coming from a previous Android version.
- If you face issues like poor RAM management or storage problems, it indicates that you have not followed the instructions or have changed the kernel/recovery. STRICTLY follow the provided instructions before reporting any issues.

**Note:** Formatting with RisingOS Recovery (yes, ONLY RisingOS Recovery) is mandatory during a clean flash.

---

# **Rom Download**
- [RisingOS-Revived](https://risingosrevived.tech/downloads.html?codename=sunny)


# **Recovery Images Download**

- [Gapps](https://sourceforge.net/projects/risingos-revived/files/6.x/GAPPS/sunny/recovery_images/)
- [Core](https://sourceforge.net/projects/risingos-revived/files/6.x/CORE/sunny/recovery_images/)
- [Vanilla](https://sourceforge.net/projects/risingos-revived/files/6.x/VANILLA/sunny/recovery_images/)


## **Installation Methods**

### 1. **SD Card Method (Most Reliable)**

1. **Download the ROM** into your SD card.
2. **Reboot the device to bootloader (Fastboot Mode).**
3. Flash the boot image:
   ```
   fastboot flash boot <path/to/boot.img>
   ```
4. Flash the vendor_boot image:
   ```
   fastboot flash vendor_boot <path/to/vendor_boot.img>
   ```
5. **Reboot to Recovery.**
6. **Format data** and reboot recovery.
7. Apply update > Flash firmware `14.0.9.0` > Reboot to Recovery.
8. Apply update > Flash downloaded ROM > Reboot to System.

**For Dirty Flash:**
Go to **Update from SD Card** > Apply Update > Flash ROM.

---

### 2. **Clean Flash (Coming from a Different ROM)**

> **Note:** Clean flash involves formatting data, which means you will lose data stored in the internal storage of your device. Data in the SD card should not be affected. I will not be responsible for any loss of data.

1. **Download the ROM, vendor_boot, and boot files** to your computer (click on the recovery button for vendor_boot and boot).
2. **Reboot the device to bootloader (Fastboot Mode).**
3. Flash the vendor_boot image:
   ```
   fastboot flash vendor_boot <path/to/vendor_boot.img>
   ```
4. Flash the boot image:
   ```
   fastboot flash boot <path/to/boot.img>
   ```
5. Reboot to recovery:
   ```
   fastboot reboot recovery
   ```
6. In Recovery Mode:
   - Go to **Main Menu > Factory Reset > Format Data/Factory Reset > Format Data**.
   - Return to the **Main Menu** > Reboot to Recovery.
7. On your phone (in recovery mode):
   - Apply Update > Apply from ADB.
8. Flash the ROM via ADB sideload:
   ```
   adb sideload <path/to/rom.zip>
   ```
9. Flash firmware (Version `V14.0.9.0.SKGMIXM`) via ADB sideload:
   ```
   adb sideload <path/to/firmware.zip>
   ```
10. **Reboot and enjoy!**

---

### 3. **Dirty Flash / Update**

> **Note:** There will be no loss of data if everything goes well. Keep backups in case of any mishap. I will not be responsible for any loss of data.

1. **Download the ROM file** to your computer.
2. **Reboot the device to Recovery.**
3. On your phone (in recovery mode):
   - Apply Update > Apply from ADB.
4. Flash the ROM via ADB sideload:
   ```
   adb sideload <path/to/rom.zip>
   ```
5. Flash firmware (Version `V14.0.9.0.SKGMIXM`) via ADB sideload:
   ```
   adb sideload <path/to/fw.zip>
   ```
6. **Reboot and enjoy**

