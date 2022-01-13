+++
title = "Odysseyn1x"
date = "2022-01-11T23:11:06-05:00"
author = "stkc"
authorTwitter = "atoiletcat" #do not include @
cover = ""
tags = ["odysseyn1x", "checkra1n"]
keywords = ["odysseyn1x", "checkra1n"]
description = "Use Odysseyra1n on any computer using a USB flash drive."
showFullContent = false
readingTime = false
+++

![Odysseyn1x logo](odysseyn1x-logo.png)\
\
Odysseyn1x is a miniature Linux distribution that allows users to easily jailbreak their devices with checkra1n. Maintained by [raspberryenvoie](https://github.com/raspberryenvoie).

We will be using Ventoy rather than Rufus or Etcher since not only is it easier, you can continue you use your USB drive to store files while still being able to boot Odysseyn1x.

If you have a Ryzen processor it's very likely the jailbreak will fail repeatedly, use an Intel machine if possible.

# Requirements

[Odysseyn1x](https://github.com/raspberryenvoie/odysseyn1x/releases)
- *Download `amd64` if you are on a 64-bit computer, otherwise use `i686`.*
- *If you are using a device with an A9X processor, use [this](https://github.com/asdfugil/checkn1x_a9x_kerninfo_pongoOS/releases/tag/14.5-a9x-2) fork of Odysseyn1x.*

[Ventoy](https://github.com/ventoy/Ventoy/releases)

# Installing Ventoy

![Extracted in Explorer](extracted-explorer.png)

After downloading and extracting the Ventoy .zip file, connect your USB flash drive then open the `Ventoy2Disk.exe` program.

Now is the time to copy any important files to another drive. You can copy them back after the installation.

![Ventoy Window](ventoy-before-install.png)

Select your USB flash drive at the top then press `Install`. You will be prompted twice to confirm that you are okay with deleting all data on the drive. *(You backed up your files, right?)*

If successful, the version number for `Ventoy In Package` should match `Ventoy In Device`.

Now open File Explorer and select the new `Ventoy` USB device.

![Ventoy in File Explorer](ventoy-usb-on-drive.png)

Copy the Odysseyn1x .iso file to the drive. If you'd like to keep everything organized you can make a folder and put the .iso inside that.

You can move your old files back on to the USB flash drive now if necessary.

# Preparing to boot Odysseyn1x

Before we can boot directly into Odysseyn1x we will need to do two things: disable Secure Boot and change the boot order.

Entering the BIOS is different on every computer. Refer to [this list](https://www.disk-image.com/faq-bootmenu.htm) to find the correct key to press. If you don't see your computer try pressing the function keys (F1, F2, etc.) or ESC, DEL or Enter immediately after powering on your computer.

After entering the BIOS look for `Secure Boot` and set it to `Disabled`. It is usually located in the `Security` or `Boot` tab. 

If you cannot change this option you may need to set a BIOS or "Administrator" password. Make sure you don't forget this otherwise you can get permanently locked out of the BIOS.

Now look for `Boot Option` or `Boot Order`. Move your USB flash drive to the top of the list or set it as the first option. Usually it will show the drive's model or brand name however it may only show as `USB Hard Disk`.

Make sure you save and exit.

# Booting Odysseyn1x

If you set your boot order correctly you will be loaded into the Ventoy boot menu. Otherwise, press the boot menu key immediately after powering on your computer and select the USB flash drive.

![Ventoy boot menu](ventoy-bootscreen.png)

Press Enter and you will be loaded into the Odysseyn1x menu.

![Odysseyn1x menu](odysseyn1x-menu.png)

# Jailbreaking

Now for the fun part, select `Checkra1n` and follow the instructions on screen.
- *If you see "Sorry, [device] is not supported on [iOS version] at this point." select `Options` and enable `Allow untested iOS/iPadOS/tvOS versions`.*
- *If you still cannot continue, and you are using an A11 device, disable your passcode and enable `Skip A11 BPR check`.*

If succesful, your device will boot and the checkra1n app will appear on your homescreen. **Do not open it!**

# Installing Odysseyra1n

We will be installing Odysseyra1n as it comes with up-to-date core utilities, an actively maintained package manager, and a more efficient tweak injection library.

Select `Quit` in checkra1n, then on the Odysseyn1x menu select `Odysseyra1n`.

With your device still connected, press enter and then follow the on-screen prompts.
- *If you see "Failed to install Procursus bootstrap and Sileo on your device." you may not have successfully jailbroken, repeat the jailbreaking steps. If you continue to get errors, you can try running [this shortcut](https://go.stkc.win/shortcut) directly on your device.*

Sileo will appear on your homescreen. This is the modern alternative to Cydia and supports the same tweaks and repos. Open it then navigate to the `Packages` tab. Select `Upgrade All` and restart SpringBoard if prompted.

If you wish to use Cydia you can search for `Cydia Installer` within Sileo and optionally uninstall Sileo afterwards. Installing it from the checkra1n app will **ruin your jailbreak!**

# You're done!

Select `Shut down` within Odysseyn1x then unplug your USB flash drive. You can now boot your computer back into Windows.

When your phone's battery dies or if you reboot you will need to rerun the jailbreak, this is because checkra1n is semi-tethered. Simply select `Checkra1n` in the Odysseyn1x menu and repeat the steps you followed earlier. You do not need to run `Odysseyra1n` again, this is a one-time install script.

# Still need help?

Join the [r/Jailbreak](https://discord.gg/jb) or [Sileo](https://discord.gg/sileo) Discord servers.