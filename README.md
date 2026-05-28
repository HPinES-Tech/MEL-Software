# MEL Software
MEL Software (Minecraft Experience Launcher Software) is a tool that can play Minecraft Bedrock on your Android phone via computer.

![Play Minecraft on Phone via PC](https://github.com/HPinES-Tech/MEL-Software/blob/main/Play%20Mincraft%20in%20phone%20via%20PC.png?raw=true)
NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.

# ⚠️ WARNING!
Before installing this tool, you must know that we think you live under a rock and that:
- This tool is **NOT** yet available on Apple devices due to software limitations.
- This tool is in stages of **ALPHA.** It's not fully stable. You can head down to the [Troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.
- This tool is **NOT** a virus. It is 100% safe to use since the .bat file only runs scrcpy, adb, and echo commands. It does not forward your data to any server.
    - If Windows says it could be a virus, do not trust it, in the meantime, you can check out [our VirusTotal scan](https://www.virustotal.com/gui/file/e46405c06f369cebe30e177e400b732bbd2c00d8a2c13b1f1f98dd87b01e9900?nocache=1). (will be updated regularly on each updates)
        - If you're full of shit and paranoia, then you can run the scan yourself by downloading the .ZIP file on Github your own, fuck you.
- This tool can have a long time updating due to Linux distributions support and timezones, we cannot set a release date for the later versions because we might delay it over and over...
- If you unplug your phone during the session, then it is not our fault that your phone has the highest resolution all of the sudden. (does not mean it's a virus, you're just an idiot and that's your problem)
    - To exit the tool, please close the application that is displaying Minecraft (by pressing ALT+F4), your phone display settings will be reverted back to normal, this is recommended to do so.
    - If your phone has been affected with the highest resolution, then please head down the [troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.

Download this software [here](https://github.com/HPinES-Tech/MEL-Software/releases/tag/v1.0.0-alpha.2)

This warning section will be removed once we move onto a stable release. Our whole guide is in the [Wiki section](https://github.com/HPinES-Tech/MEL-Software/wiki) of this Github page.

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

macOS (Intel):
If you're having trouble trying to open it, try launching it again, it can sometimes fail due to the hardware limitations.

# Contributor's role:
- HPinES Tech: This person's role is to write software in CLI format, create/edit README.md and "Releases" containing software descriptions, and upload them. This person add Linux and Windows legacy support.
- peanutsloveem: This person's role is to write software in Graphics UI format, create/edit README.md and "Releases" containing software descriptions, and upload them. This person adds MacOS and modern Windows support.

**To receive the best support, contact the right person for the software bug you are using (one of the two contributors).**
