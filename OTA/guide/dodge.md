# RisingOS Installation Instructions
-------------------------------
 
### **Installation Methods**

***Oneplus 13 Dodge***

## **Clean Flash Steps:**

• Flash Important .img files via Bootloader
    - fastboot flash boot boot.img
    - fastboot flash dtbo dtbo.img
    - fastboot flash recovery recovery.img
    - fastboot flash vendor_boot vendor_boot.img
    
•Reboot To Recovery

## Flash via adb:**

•Wipe data

•Flash the ROM via ADB sideload:
   ```
 adb sideload <path/to/rom.zip>

• Reboot to System

"Profit"

---

## Dirty flash:**

• Adb reboot recovery

• Flash the ROM via ADB sideload:
   ```
   adb sideload <path/to/rom.zip>

• Reboot to system

---


