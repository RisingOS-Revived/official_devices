==================================================
        RisingOS Revived - Installation Guide
==================================================

Maintainer: SenX
Device: [MUNCH]
==================================================

!! READ THIS FIRST !!

- Backup your personal data before starting.
- Use the latest OrangeFox Recovery (OFOX) or TWRP.
- Make sure you are on the latest device firmware.
- Clean flash is REQUIRED if you are switching ROMs or Android versions.
- Dirty flash is possible but at your own risk.
- I am not responsible for any damage or data loss.

--------------------------------------------------

GAPPS and CORE VARIANT (CLEAN FLASH)

1. Reboot to Recovery.
2. Wipe Dalvik/Cache, Metadata, and Data.
3. Flash Firmware (skip if included).
4. Flash RisingOS ROM.
5. Flash TWRP/OrangeFox Recovery 
   (only if you want to keep custom recovery instead of ROM’s default).
6. Reboot back to Recovery.
7. Format Data (type YES).
8. Reboot to System.

--------------------------------------------------

VANILLA (CLEAN FLASH)

1. Reboot to Recovery.
2. Wipe Dalvik/Cache, Metadata, and Data.
3. Flash Firmware (skip if included).
4. Flash RisingOS ROM.
5. Flash TWRP/OrangeFox Recovery 
   (only if you want to keep custom recovery instead of ROM’s default).
6. Reboot back to Recovery.
7. Flash GApps (Core/Full) or MicroG (optional).
8. Format Data (type YES).
9. Reboot to System.

--------------------------------------------------

DIRTY FLASH (Update / Same Base):

1. Backup your data (precaution).
2. Boot into Recovery.
3. Flash RisingOS Revived ROM.
4. Flash TWRP/OrangeFox Recovery 
   (only if you want to keep custom recovery instead of ROM’s default).
5. Wipe ONLY:
   - Dalvik / ART Cache
   - Cache
6. If using VANILLA build, flash GApps (Core/Full) or MicroG.
7. Reboot to System.

*Note: Dirty flashing keeps data, but always have backups in case.*

--------------------------------------------------

FLASH VIA ADB SIDELOAD:

1. Backup your files.
2. Connect device to PC.
3. Boot into Recovery using:
   adb reboot recovery
4. In recovery, select ADB sideload option.
5. On PC, run:
   adb sideload <path/to/rom.zip>
6. Wait for the process to finish, then reboot.

--------------------------------------------------

TIPS & NOTES:

- Always update to the latest recovery before flashing.
- Bugs like poor RAM handling or storage issues usually mean
  you did not follow instructions correctly.
- Clean flash is REQUIRED if you come from another ROM or
  previous Android version.
- If you want to keep custom recovery (TWRP/OFOX), 
  re-flash it after flashing the ROM.

==================================================
     End of Guide – Flash at your own risk
==================================================
