# MEL Software
MEL Software (Minecraft Experience Launcher Software) is a tool that can play Minecraft Bedrock on your Android phone via computer.

![Play Minecraft on Phone via PC](https://github.com/HPinES-Tech/MEL-Software/blob/main/Play%20Mincraft%20in%20phone%20via%20PC.png?raw=true)
NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.

# WARNING!
Before installing this tool, you must know that:
- This tool is **NOT** yet available on Apple devices due to software limitations.
- This tool is in stages of **ALPHA.** It's not fully stable. You can head down to the [Troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.
- This tool is **NOT** a virus. It is 100% safe to use since the .bat file only runs scrcpy, adb, and echo commands. It does not forward your data to any server.
    - If Windows says it could be a virus, do not trust it, in the meantime, you can check out our VirusTotal scan. (will be updated regularly)
        - If you're full of shit and paranoia, then you can run the scan yourself by downloading the .ZIP file on Github your own, fuck you.
- This tool can have a long time updating due to Linux distributions support and timezones, we cannot set a release date for the later versions because we might delay it over and over...
- If you unplug your phone during the session, then it is not our fault that your phone has the highest resolution all of the sudden. (does not mean it's a virus)
    - To exit the tool, please close the application that is displaying Minecraft, your phone display settings will be reverted back to normal, this is recommended to do so.
    - If your phone has been affected with the highest resolution, then please head down the [troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.

Download this software [here](https://github.com/HPinES-Tech/MEL-Software/releases/tag/v1.0.0-alpha.2)

This warning section will be removed once we move onto a stable release.

# Installation guide
- Windows:
  + G-UI: Unzip the .zip file to a folder and open MEL-Software.exe, run it as administrator.
  + CLI: (soon...) Unzip the .zip file to a folder and run Launcher.bat

- macOS:
If you are running any version that's lower than macOS 13, go to the [MacPorts Guide](https://guide.macports.org/) and download your version, update it every once in a while. And then type the commands below into the terminal:
```bash
# You need to download Homebrew in order for this to work.
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"

# And then you can download the rest.
brew install android-platform-tools
brew install scrcpy

# If the adb commands is not found after install then enter the following commands below.

# Intel Macs
echo 'export PATH="/usr/local/bin:$PATH"' >> ~/.zshrc
source ~/.zshrc

# For Apple Sillicon
echo 'export PATH="/opt/homebrew/bin:$PATH"' >> ~/.zshrc
source ~/.zashrc

# And then make executable clickable
chmod +x dir/to/the/Minecraft Experience Launcher/dist/MEL-Software
```

- Linux:
  + GUI: Not there yet.
  + CLI: soon...

# Testing
This is all the following Android devices and computers that we have tested on, and what version of MEL and MCPE did we test it on.

- Androids:
  - Nothing Phone (2a)
    - Model: A142
    - Chipset/CPU: Mediatek Dimensity 7200 Pro
    - GPU: Mali-G610 MC4
    - RAM: 8 GB of RAM (RAM Booster: +4 GB) 
    - OS: NothingOS 4.0 (Android 16)
    - MCPE Version: 26.13 (1.26.13.1 – 1.26.14.1)
    - MEL Version: v1.0.0-alpha.2
  - Samsung Galaxy S23 FE
    - Model: SM-S711B
    - Chipset/CPU: Samsung Exynos 2200
    - GPU: Xclipse 920
    - RAM: 8 GB of RAM
    - OS: OneUI 7.0 (Android 15)
    - MCPE Version: 1.21.131
    - MEL Version: v1.0.0-alpha.1
  - Samsung Galaxy Note 9
    - Model: SM-N960N
    - Chipset/CPU: Samsung Exynos 9810
    - GPU: ARM Mali-G72 MP18
    - RAM: 6 GB of RAM
    - OS: Noble ROM 4.3 CALABRIA - OneUI 6.1.1 (Android 14)
    - MCPE Version: 1.21.131
    - MEL Version: v1.0.0-alpha.1
  - Huawei Nova 2 Plus
    - Model: BAC-TL00
    - Chipset/CPU: Kirin 659
    - GPU: Mali-T830 MP2
    - RAM: 4 GB of RAM
    - OS: EMUI 8.0.0 (Android 8)
    - MCPE Version: 1.19.83
    - MEL Version: Alpha v1.0.0.2

- OSes:
    - Windows
      - Windows 11 25H2 - Home (AtlasOS)
        - CPU: Intel 11th Generation Core i5-11400H
        - GPU: Nvidia GeForce GTX 1650 with Max-Q Design
        - RAM: 8 GB of DDR4
        - Version: v1.0.0-alpha.2
      - Windows 10 22H2 - Home Single Language
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3
        - Version: v.1.0.0-alpha.1
      - Windows 7 - Ultimate (requires [Vxkex](https://github.com/i486/VxKex) to use)
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3
        - Version: v.1.0.0-alpha.2

    - Linux
      - Xubuntu 24.04.2 LTS (Xfce)
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3
        - Version: v.1.0.0-alpha.1
      - Linux Mint Cinnamon 22.1 (GNOME)
        - CPU: Intel Pentium N3710
        - GPU: Intel HD Graphics 405
        - RAM: 8 GB of DDR3
        - Version: v.1.0.0-alpha.1
       
    - macOS
      - macOS Monterey (version 12.7.6)
        - Model: A1708 (MacBook Pro (13-inch, 2017, Two Thunderbolt 3 ports))
        - CPU: Dual-Core Intel Core i5
        - GPU: Intel Iris Graphics 520
        - RAM: 8 GB of LPDDR3
        - Version: v1.0.0-alpha.2

Many OSes will be added soon later in the future. For now, contact one of our (two) contributors if you have tested it on different builds of OSes and other models of Android phones.

# Usage
- Android: Enable "USB Debugging" in Settings, and allow your PC to make changes.
- Windows: Extract the .zip file into anywhere ("\Documents" is recommended) and run "Launcher.bat"
  - For Windows 7, you must use [Vxkex](https://github.com/i486/VxKex) to run the .exe file (G-UI version), because it has reached end of support for modern apps. (Not needed with CLI version)
- Linux GNOME: Extract the .zip file into anywhere ("\Documents" is recommended) and run "Launcher(.desktop)"
- Linux Xfce: Extract the .zip file into anywhere ("\Documents" is recommended) and run "Launcher.desktop"

  + On Windows, make sure you installed [Google USB Driver](https://developer.android.com/studio/run/win-usb?hl=vi) for Android Devices or [Samsung Android USB Driver](https://developer.samsung.com/android-usb-driver) for Samsung Devices.

# Troubleshooting
Android: Go to developer settings and change the DPI to your device's normal DPI (one quick Google search)

Windows/Linux/macOS (using adb):
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

macOS:
If you're having trouble trying to open it, try launching it again. This can happen because scrcpy failed to open, and you must try again.

# Contributor's role:
- HPinES Tech: This person's role is to write software in CLI format, create/edit README.md and "Releases" containing software descriptions, and upload them. This person add Linux and Windows legacy support.

- peanutsloveem: This person's role is to write software in Graphics UI format, create/edit README.md and "Releases" containing software descriptions, and upload them. This person adds MacOS and modern Windows support.

  + *To receive the best support, contact the right person for the software bug you are using (one of the two contributors).*
