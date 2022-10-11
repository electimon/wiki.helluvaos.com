---
sidebar_label: A-Only
---

# A-Only Installation Guide

## Before you start
1. ** Keep a backup of your data.** Make sure to keep a backup of your files as the installaton will wipe your data.

2. ** You must come from MIUI.** Make sure you come from MIUI and not using other ROM before installation. If you come from other ROM, flash MIUI and boot it once before continuing installation.

## Connect your device

1. **Enter Fastboot mode,** make sure your phone turned off. Press and hold the Power and Volume buttons for 3 seconds until the phone turns on. You will be in Fasboot mode.

   ![Fastboot](/img/install-assets/fastboot.svg)

2. Once your phone is in Fastboot mode, connect your phone to a computer using a USB Cable.
3. Once you connected your phone to a computer using a USB Cable, check your phone connection to the computer by executing `fastboot devices`
4. Once the device showed up in fastboot devices, continue with Sideloading the boot image with the following commands:
``` bash
fastboot flash dtbo dtbo_gourami.img
fastboot flash recovery recovery_DEVICENAME.img
```
## Install from MIUI

1. **Enter Recovery mode** by pressing and holding the Power and Volume up buttons for 3 seconds until the phone turns on. You will be in Recovery mode.
2. Once your phone is in Recovery mode and shows “No Command”, hit Power button, while holding it, hit Volume + (Up) button.

    ![KeyCombination](/img/install-assets/key-combination.svg)

3. **Do a Factory Reset.** Use the volume buttons to move through the menu options, when “Factory Reset” is highlighted, press the Power button.

    ![WipeData](/img/install-assets/wipe-data.svg)

4. Use the volume buttons to move through the menu options, when “Install update through ADB” is highlighted, press the Power button.

    ![ADBInstall](/img/install-assets/adb-install.svg)

5. Flash the ROM through recovery with adb sideload command from your Mac/PC.

    ![ADBSideloadWindow](/img/install-assets/adb-sideload-window.svg)

6. Use the volume buttons to move through the menu options, when “Reboot to System” is highlighted, press the Power button.

    ![Reboot to System](/img/install-assets/reboot-system.svg)

# Sideloading Updates

1. **Enter Recovery mode** by pressing and holding the Power and Volume up buttons for 3 seconds until the phone turns on. You will be in Recovery mode.
2. Once your phone is in Recovery mode and shows “No Command”, hit Power button, while holding it, hit Volume + (Up) button.

    ![KeyCombination](/img/install-assets/key-combination.svg)

3. Use the volume buttons to move through the menu options, when “Install update through ADB” is highlighted, press the Power button.
4. Flash the ROM through recovery with adb sideload command from your Mac/PC.

    ![ADBSideloadWindow](/img/install-assets/adb-sideload-window.svg)
5. Use the volume buttons to move through the menu options, when “Reboot to System” is highlighted, press the Power button.