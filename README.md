# Moto-G-Play-2024-GSI-Guide-and-Tutorial
GSI guide for Moto G Play 2024 

Hello! This is a guide mainly for the Moto G Play series phones. Specifically for GSIs for them.

Prerequisites & Tools
Why GSIs? The main reason I'm using a GSI on this specific device is due to the 
- Hardware: Moto G Play (2024) reliable USB-C cable and a PC that can run Android ADB Platform-Tools.
- Android Platform-Tools: You will need the latest platform-tools; you can find it at https://developer.android.com/tools/releases/platform-tools
- Motorola USB Drivers: You can also find these at https://en-us.support.motorola.com/app/usb-drivers
- GSI Image: Any GSI will work, as GSIs are meant to be used natively on any device. For this tutorial I will be using the arm64_bgN LineageOS 21 Treble image, uncompressed `.img`, which you can find online on GitHub as   well.

Bootloader Unlock
- To begin enable Developer Options, go to Settings > About Phone > tap Build Number 7 times. Enter your PIN if needed
- In Developer Options, enable USB Debugging and OEM Unlocking.
    *Note:* If OEM Unlocking is greyed out, connect the phone to an active Wi-Fi network and check for updates to sync with Motorola's servers; this may take a while. In my case, it took 2 weeks for it to be able to be
    unlocked.

ADB Steps
- From here, make sure your platform-tools are working. Do Shift + Right-click and select Open with Microsoft PowerShell
- Now do ```bash
adb start-server
```
- 
  
