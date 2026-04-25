# MEL Software
MEL Software (Minecraft Experience Launcher Software) is a tool that can play Minecraft Bedrock on your Android phone via computer.

![Play Minecraft on Phone via PC](https://github.com/HPinES-Tech/MEL-Software/blob/main/Play%20Mincraft%20in%20phone%20via%20PC.png?raw=true)
NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.

# **WARNING!**
Before installing this tool, you must know that:
- This tool is **NOT** yet available on Apple devices due to software limitations.
- This tool is in stages of **ALPHA.** It's not fully stable. You can head down to the [Troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.
- This tool is **NOT** a virus. It is 100% safe to use since the file only runs scrcpy, adb, and echo commands. It does not forward your data to some server.

Download it here: https://github.com/HPinES-Tech/MEL-Software/releases/tag/Alpha

This warning section will be removed once we move onto a stable release.

# Testing
This is all the following Android devices and computers that we have tested on.

- Androids:
  - Samsung Galaxy Note 9
    - Model: SM-N960N
    - OS: Noble ROM 4.3 CALABRIA - OneUI 6.1.1 (Android 14)
  + Nothing Phone (2a)
    + Model: A142
    + OS: NothingOS 4.0 (Android 16)

- OSes:
    - Windows
      - Windows 10 22H2 - Home Single Language
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3
      - Windows 11 25H2 - Home (AtlasOS)
        - CPU: Intel 11th Generation Core i5-11400H
        - GPU: Nvidia GeForce GTX 1650 with Max-Q Design
        - RAM: 8 GB of DDR4
      - Windows 7 - Ultimate (requires [Vxkex](https://github.com/i486/VxKex) to use)
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3

    - Linux
      - Linux Mint Cinnamon 22.1 (GNOME)
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3
      - Xubuntu 24.04.2 LTS (Xfce)
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3

Many OSes will be added soon later in the future. For now, contact one of our (two) contributors if you have tested it on different builds of OSes and other models of Android phones.

# Usage
- Android: Enable "USB Debugging" in Settings, and allow your PC to make changes.
- Windows: Extract the .zip file into anywhere ("\Documents" is recommended) and run "Launcher.bat"
  - For Windows 7, you must use [Vxkex](https://github.com/i486/VxKex) to run the .bat file, because it has reached end of support for modern apps.
- Linux GNOME: Extract the .zip file into anywhere ("\Documents" is recommended) and run "Launcher(.desktop)"
- Linux Xfce: Extract the .zip file into anywhere ("\Documents" is recommended) and run "Launcher.desktop"

# Troubleshooting
Android: Go to developer settings and change the DPI to your device's normal DPI (one quick Google search)

Windows/Linux (using adb):
If your phone screen is severely out of order, then please use the commands below.
- For Windows: use "cd" to your directory where the Tools folder can be found, it is all you need to troubleshoot your problems

```bash
# This command lets you use your PC's keyboard/mouse on the device. (if you softlocked it)
scrcpy --otg

# This command resets the screen resolution.
adb shell wm size reset

# These commands resets the orientation type.
adb shell settings put system user_rotation 0
```
