# RisingOS Revived for the OnePlus 12 (Waffle)

# Steps to Flash: 

# Main Steps
1. Make sure to have Android's Platform Tools available
2. Boot the phone into the bootloader
3. Do fastboot -w (THIS WILL WIPE EVERYTHING!!!! MAKE SURE YOU HAVE BACKUPS OF IMPORTANT DOCUMENTS, PHOTOGRAPHS, OR OTHER IMPORTANT THINGS!!!!)
4. Download the latest recovery image in the "Recovery" folder. 
5. Do fastboot flash recovery C:\Path\to\Recovery\Image\recovery.img (You can just drag and drop the actual .img file on to the Command Prompt window or whatever you're using.).

# OTA Route
1. Download the latest OTA from the "OTA Files" folder.
2. While you're still in the bootloader, do fastboot reboot recovery.
3. When you enter the Reovery interface, use the volume keys and go down to "Apply update over ADB."
4. Click on that button with the power button and if it asks for confirmation, confirm. 
5. Do adb side load C:\Path\to\OTA\File\ota.zip (You can just drag and drop the actual file onto the window.).
6. If it asks if you want to flash anything else, tell it no. It comes with Google Applications already.
7. Reboot if it asks you to.
8. Done. Let it boot up now.

# Fastboot Route
1. Download the latest Fastboot package from the "Fastboot Files" folder.
2. While you're still in the bootloader, do fastboot reboot fastboot
3. When you see "fastbootd" on the screen, do fastboot update C:\Path\to\Fastboot\Package\fastboot.zip (You can just drag and drop on the window.).
4. Let it do its thing and then it'll reboot automatically. 
5. Done! Let it boot up now!