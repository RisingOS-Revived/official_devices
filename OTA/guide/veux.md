# RisingOS Installation Instructions

**Author:** @MrTopia

-------------------------------

## **Instructions**

### **ALWAYS Keep in Mind...**

> **Note:** Clean flash involves formatting data, which means you will lose data stored in the internal storage of your device. Data in the SD card should not be affected. I will not be responsible for any loss of data.

## When do a clean flash? Here you go...**
- You are coming from any other ROM.
- You are coming from a previous Android version.
- If you face issues like poor RAM management or storage problems, it indicates that you have not followed the instructions or have changed the kernel/recovery. STRICTLY follow the provided instructions before reporting any issues.
- Always make sure your on your devices latest google firmware 

-------------------------------
 
### **Installation Methods**

## **Clean Flash Steps:**

• Backup your Important files ( cloud / pc )

• Flash Important .img files via Bootloader
    - fastboot flash boot boot.img
    - fastboot flash dtbo dtbo.img
    - fastboot flash vendor_boot vendor_boot.img

• Boot to Recovery

• Select **Apply Update**

• Flash **RisingOS Revived** ROM

• Format Data (correct, the place where you need to type in "YES")

• Reboot and enjoy!

---

## Dirty flash:**

• Backup your Important files

• Boot to Recovery

• Flash **RisingOS Revived** ROM

• Reboot and enjoy!

> **Note:** There will be no loss of data if everything goes well. Keep backups in case of any mishap. I will not be responsible for any loss of data.

---

## OTA:**

• Go to Settings -> System -> Updater and download latest build
• Choose install and let it finish
• Reboot

---

## Flash via adb:**

• Backup your Important files

• Adb reboot recovery

• Flash the ROM via ADB sideload:
   ```
   adb sideload <path/to/rom.zip>
   ```  
