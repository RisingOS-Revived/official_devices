# RisingOS Installation Instructions
-------------------------------
 
### **Installation Methods**

## **Clean Flash Steps:**

• Flash Important .img files via Bootloader
    - fastboot flash boot boot.img
    - fastboot flash dtbo dtbo.img
    - fastboot flash recovery recovery.img
    - fastboot flash vendor_boot vendor_boot.img

• Boot to Recovery

• Flash **RisingOS Revived** ROM

• Format Data (correct, the place where you need to type in "YES")

• Reboot and enjoy!

---

## Dirty flash:**


• Boot to Recovery

• Flash **RisingOS Revived** ROM


• Reboot and enjoy!

---

## Flash via adb:**

• Backup your Important files

• Adb reboot recovery

• Flash the ROM via ADB sideload:
   ```
   adb sideload <path/to/rom.zip>
