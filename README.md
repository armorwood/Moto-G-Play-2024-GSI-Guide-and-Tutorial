# Moto-G-Play-2024-GSI-Guide-and-Tutorial
GSI guide for Moto G Play 2024 

Hello! This guide is mainly for Moto G Play series phones. Specifically for GSIs for them.

**Prerequisites & Tools**
Why GSIs? The main reason I'm using a GSI on this specific device is due to the lack of support these budget devices have. Putting a GSI is a perfect way to making it run much smoother and cleaner.
- Hardware: Moto G Play (2024), a reliable USB-C cable, and a PC that can run Android ADB Platform-Tools.
- Android Platform-Tools: You will need the latest platform-tools; you can find it at https://developer.android.com/tools/releases/platform-tools
- Motorola USB Drivers: You can also find these at https://en-us.support.motorola.com/app/usb-drivers
- GSI Image: Any GSI will work, as GSIs are meant to be used natively on any device. For this tutorial, I will be using the arm64_bgN LineageOS 21 Treble image, uncompressed `.img`, which you can find online on GitHub as   well.

**Bootloader Unlock**
- To begin, enable Developer Options, go to Settings > About Phone > tap Build Number 7 times. Enter your PIN if needed
- In Developer Options, enable USB Debugging and OEM Unlocking.
    *Note:* If OEM Unlocking is greyed out, connect the phone to an active Wi-Fi network and check for updates to sync with Motorola's servers; this may take a while. In my case, it took 2 weeks for it to be able to be
    unlocked.

ADB Steps
- From here, make sure your platform-tools are working. Do Shift + Right-click and select Open with Microsoft PowerShell
- Step 1: Run this command. **\adb start-server**
- Step 2: Run **\adb devices** and make sure your device is listed, that you've enabled USB debugging, and that it is authorized. If it isn't, revoke it in the Developer Options menu, then unplug and plug it back in until     you allow it.
- Step 3: Run **\adb reboot bootloader**, to check if it is recongized run **\fastboot devices**
- Step 4: Run **fastboot oem get_unlock_data** it should return back in this format **fastboot oem unlock <YOUR_UNLOCK_KEY>**
- Step 5: Head to 

  
