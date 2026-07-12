Flashing Guide for Redmi Note 9 Pro / Pro Max / 9S / POCO M2 Pro (miatoll)

Clean Flash (Recovery)
1. Boot into the recommended recovery.
2. Go to Apply Update > Apply from ADB.
3. Flash the ROM:
   adb sideload ROM-*.zip
4. Once the installation is complete, reboot back to recovery.
5. If you're using the Vanilla build, sideload your preferred GApps package (optional).
6. Format Data / Factory Reset.
7. Reboot to System.

Note: The first boot may take a few minutes.

Clean Flash (Fastboot)
1. Boot your device into Fastboot mode.
2. Flash the required images:
   fastboot flash recovery recovery.img
   fastboot flash vendor_boot vendor_boot.img
3. Reboot into recovery:
   fastboot reboot recovery
4. Go to Apply Update > Apply from ADB.
5. Flash the ROM:
   adb sideload ROM-*.zip
6. Reboot back to recovery.
7. If you're using the Vanilla build, sideload your preferred GApps package (optional).
8. Format Data / Factory Reset.
9. Reboot to System.

Dirty Flash (Previous Build)
Only supported when updating from an older build of the same ROM.
1. Boot into recovery.
2. Go to Apply Update > Apply from ADB.
3. Flash the latest ROM:
   adb sideload ROM-*.zip
4. Reboot back to recovery.
5. If required, sideload GApps again (Vanilla build only).
6. Reboot to System.

Notes
• Clean flash is required when switching from another ROM.
• Dirty flash is only recommended when updating from a previous build of the same ROM.
• First boot can take 5–10 minutes.
