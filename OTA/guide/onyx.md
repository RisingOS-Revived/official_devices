Flashing instructions for Poco F7 (onyx)


CLEAN FLASH:

1. Flash the provided recovery image and vendor boot image via fastboot using "fastboot flash recovery recovery.img" & "fastboot flash vendor_boot vendor_boot.img"
2. Reboot to recovery using either volume + and power button combo or via fastboot command
3. Navigate to Apply Update > Apply from ADB
4. adb sideload the AOSP ROM zip using "adb sideload ROM-*.zip"
5. Reboot to recovery
6. Vanilla Build user who want flash gapps using  "adb sideload gapps-*.zip" (optional)
7. Factory reset/format data
8. Reboot to system


DIRTY FLASH:

1. Go to recovery
2. Navigate to Apply Update > Apply from ADB
3. adb sideload the AOSP ROM zip using "adb sideload ROM-*.zip"
4. Reboot to recovery
5. Vanilla Build user who want flash gapps using  "adb sideload gapps-*.zip" (optional)
6. Reboot to system


