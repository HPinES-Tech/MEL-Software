# MEL Software
MEL Software (Minecraft Experience Launcher Software) is a tool that can play Minecraft Bedrock on your Android phone via computer.

![Play Minecraft on Phone via PC](https://github.com/HPinES-Tech/MEL-Software/blob/main/Play%20Mincraft%20in%20phone%20via%20PC.png?raw=true)
NOT AN OFFICIAL MINECRAFT PRODUCT. NOT APPROVED BY OR ASSOCIATED WITH MOJANG OR MICROSOFT.

# ⚠️ WARNING!
Before installing this tool, you must know that we think you live under a rock and that:
- This tool is **NOT** yet available on iPhone devices due to software limitations.
- This tool has **NOT** been tested or ran on an Apple Silicon device, therefore, it is not recommended to do so.
- This tool is in stages of **ALPHA.** It's not fully stable. You can head down to the [Troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.
- This tool is **NOT** a virus. It is 100% safe to use since the .bat file only runs scrcpy, adb, and echo commands. It does not forward your data to any server.
    - If Windows says it could be a virus, they said "it could be" without actually checking if there's a virus or not. In the meantime, you can check out [our VirusTotal scan](https://www.virustotal.com/gui/file/e46405c06f369cebe30e177e400b732bbd2c00d8a2c13b1f1f98dd87b01e9900?nocache=1). (will be updated regularly on each updates)
- This tool can have a long time updating due to Linux distributions support and timezones, we cannot set a release date for the later versions because we might delay it over and over... *or we're just lazy...*
- This tool may or may not ask Claude AI for code samples throughout the coding experience. (@peanutsloveem)
- If you unplug your phone during the session, then it is not our fault that your phone has the highest resolution all of the sudden. (does not mean it's a virus, you're just an idiot and that's your problem)
    - To exit the tool, please close the application that is displaying Minecraft (by pressing ALT+F4), your phone display settings will be reverted back to normal, this is recommended to do so.
    - If your phone has been affected with the highest resolution, then please head down the [troubleshooting section](https://github.com/HPinES-Tech/MEL-Software#troubleshooting) to fix it.
- If you think this is a virus, then you shouldn't be on Github in the first place.

This warning section will be removed once we move onto a stable release. Our whole guide is in the [Wiki section](https://github.com/HPinES-Tech/MEL-Software/wiki) of this Github page.
Download this software [here](https://github.com/HPinES-Tech/MEL-Software/releases/tag/v1.0.0-alpha.2)

# ⚙️ Troubleshooting
Android: Go to developer settings and change the DPI to your device's normal DPI (one quick Google search)

🪟/🐧/🍎 - Windows/Linux/macOS (using adb):
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

🤖 Android:
Sometimes, resetting the DPI does not work, and you will have to revert it your own by turning on Developer Mode by going to Settings > About Device/Phone > tapping the build number 7 times in a row and enter your password. One quick Google search on about your device's DPI, then go back, System > Developer options, scroll down until you see the option "Smallest width" and set it to your phone's DPI's origianl number. AS for the Nothing Phone (2a) (which I currently have) is 412 dp, so I'll put it 412. And that's it.

🍎 macOS (Intel):
If you're having trouble trying to mirror it via scrcpy, try launching it again, it can sometimes fail due to the hardware limitations.

# 👔 Contributor's J*b
- HPinES Tech: This person's role is to write software in CLI format, create/edit README.md and "Releases" containing software descriptions, and upload them. This person adds Linux, macOS and Legacy/Modern Windows support.
- peanutsloveem: This person's role is to write software in Graphics UI format, create/edit README.md and "Releases" containing software descriptions, and upload them. This person adds macOS and modern Windows support.

**To receive the best support, contact the right person for the software bug you are using (one of the two contributors).**
