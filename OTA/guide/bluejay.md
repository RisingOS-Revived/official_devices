# RisingOS Installation Instructions

**Author:** objecting_

-------------------------------

## **Instructions**

### **ALWAYS Keep in Mind...**

> **Note:** Clean flash involves formatting data, which means you will lose data stored in the internal storage of your device. Data in the SD card should not be affected. I will not be responsible for any loss of data.

## When do a clean flash? Here you go...**
- You are coming from any other ROM or MIUI.
- You are coming from a previous Android version.
- If you face issues like poor RAM management or storage problems, it indicates that you have not followed the instructions or have changed the kernel/recovery. STRICTLY follow the provided instructions before reporting any issues.

## Warning for people on April patch
- The may patch has a ARB, that can cause hard brick if not flashed correctly
- Here is how you flash it
- First flash the bootloader to **BOTH** slots with "fastboot flash bootloader path/to/image --slot all"
- Next flash your radio images to both slots with "fastboot flash radio path/to/radio --slot all
- Then flash "boot" "dtbo" and "vendor_boot", If those files are not provided, use the LineageOS files, and flash the RisingOS zip
-------------------------------
 
### **Installation Methods**

## **Clean Flash Steps:**

• Backup your Important files

• Boot to Recovery

• Flash **RisingOS Revived** ROM

• Format Data (correct, the place where you need to type in "YES")

• Flash GApps of your choice (if you have Vanilla Build)

• Reboot and enjoy!

---

## Dirty flash:**

• Backup your Important files

• Boot to Recovery

• Flash **RisingOS Revived** ROM

• Flash GApps of your choice (if you have Vanilla Build)

• Reboot and enjoy!

> **Note:** There will be no loss of data if everything goes well. Keep backups in case of any mishap. I will not be responsible for any loss of data.

---

## Flash via adb:**

• Backup your Important files

• Adb reboot recovery

• Flash the ROM via ADB sideload:
   ```
   adb sideload <path/to/rom.zip>
   ```  
