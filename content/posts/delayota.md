+++
title = "Delay OTA - Jailbroken"
date = "2022-01-14T17:58:40-05:00"
author = "flower"
authorTwitter = "" #do not include @
cover = ""
tags = ["delayota", "jailbroken"]
keywords = ["delayota", "jailbroken"]
description = "You can update using DelayOTA to versions for up to 90 days after a new version is released."
showFullContent = false
readingTime = false
+++

![delayota](dela.png)

You can update using DelayOTA to versions for up to 90 days after a new version is released.
- *This will **NOT** need any sort of Blob, it acts like a normal OTA update you'd see in settings.*

Thank you, [DhinakG](https://github.com/dhinakg/) for discovering this awesome method!

- *Note that the Alternative method **may** never work anymore once everything below `15.2` isn't availible with DelayOTA.*

# Requirements

---

1. Jailbroken Device

2. iOS 11+
- *If you're not sure on what iOS version you're currently on go to:*

`Settings` -> `General` -> `About` *and look at `Software Version`.*

If you don't have a Jailbroken device go **[here](https://guides.stkc.win/posts/delayotajailed/)**.
- *You will need to **wipe** your device when you supervise if you're unjailbroken, so we suggest you take a backup while unsupervised. Either using `iTunes/Finder`, `iMazing`, `Apple configurator 2`, or using an `iCloud Backup`.*

# Using alternate profiles

---

If you're on `14.4.2` and **lower** you need to do some extra steps before using these profiles. See: [Upgrading using Alternate profiles](#jailbroken-using-alternate-profiles-hard).
- *If you're on any `13.X` version there's a really high chance this will **NOT** work for you.*

If you're on `14.5` and **higher** we recommend following the normal method.
- *If you're having trouble join the [r/Jailbreak discord](https://discord.gg/jb) for help.*

# For Jailbroken devices `Easiest`

---

- Before we begin, make sure you add these repos: `https://cydia.ichitaso.com/` & `https://repo.cadoth.net/` to your package manager (i.e `Cydia` or `Sileo`).

Install `supervised enabler` in your package manager. 

- *This will **Supervise** your device, you will **NEED** this if you wanna DelayOTA*

Then install the profile you want to go to **[here](https://dhinakg.github.io/delayed-otas.html)**.

- *If you have an iPhone `12` or `13`, please use the `iOS (iPhone 12 series/13 series only)` section.*

- *If you have an iPhone `11` or **older** device, please use the `iOS (all other non-legacy devices)` section.*

- *This website will show the current available versions right away.*

Go to settings and search for the profile, go to:

`Settings` -> `General` -> `Profiles & Device Management`

Press on **install** when you select the profile. 

- *If it shows that it's `Not Signed` ignore it.*

**[Restore RootFS](#heading)** before upgrading, to ensure **nothing messes up** when you update. (This wont erase any personal data i.e photos & messages).

Go into Settings and see if the update is there:

`Settings` -> `General` -> `Software Update`

- *If the update is has an **error** or it says that it's **Up to Date**, please install `OTAEnabler` in your package manager*.

- *If you're using **unc0ver**, please **[Restore RootFS]()** a second time but with `Automatic Software Updates` enabled*.

Press `Download and Install`, and **[You're Done](#youre-done)**!

#

> Restore RootFS

- **Unc0ver**

Reboot, open unc0ver. Tap the gear icon and enable the Restore RootFS toggle, then tap Restore RootFS at the main screen.

---

- **Chimera / Odyssey / Taurine**

Reboot, open Chimera / Odyssey / Taurine. Toggle on Restore RootFS, then tap Jailbreak.

---

- **Checkra1n / Odysseyra1n**

Open the checkra1n app on your home screen and tap Restore System. 

- *If the icon has disappeared or you get Restore Error: General, reboot and re-jailbreak and try again.*

# Jailbroken: using alternate profiles `Hard`

---

Go through the **[For Jailbroken devices]()** section, and only install `supervised enabler`.

- *This will **Supervise** your device, you will **NEED** this if you wanna do this method*.

Install an iOS beta profile, we recommend installing **[This profile](https://cydia.ichitaso.com/no-ota15.mobileconfig)**.

Now, get an Alternate profile you'd want to upgrade to **[here](https://dhinakg.github.io/delayed-otas.html)**.

- *If you have an iPhone `12` or `13`, please use the `iOS (iPhone 12 series/13 series only)` section.*

- *If you have an iPhone `11` or **older** device, please use the `iOS (all other non-legacy devices)` section.*

- *This website will show the current available versions right away.*

Go to settings and search for the profiles, go to:

`Settings` -> `General` -> `Profiles & Device Management`

Press on **install** on both profiles. 

- *If it shows that it's `Not Signed` ignore it.*

Now, you'll need to edit a plist included in the Beta Profile, choose a method you prefer below.

> Editing the .plist

- **Using Terminal**

Install `NewTerm 2`.

- *From `https://repo.chariz.com/`.*

Install `plutil`, it should be included in your default repos.

Now, go into NewTerm 2 and paste in: 

`plutil -key MobileAssetAssetAudience -string c724cb61-e974-42d3-a911-ffd4dce11eda "/Library/Managed Preferences/mobile/com.apple.MobileAsset.plist"`

---

- **Using Filza**

Install `Filza File Manager 64-bit`.

- *From `https://tigisoftware.com/cydia`.*

If you’re reading this guide in Safari, click **[here](<filza://Library/Managed Preferences/mobile/com.apple.MobileAsset.plist>)** to navigate to the directory.

- *Otherwise, go there manually in Filza: `/Library/Managed Preferences/mobile/`.*

Set `MobileAssetAssetAudience` to `c724cb61-e974-42d3-a911-ffd4dce11eda`

---

Once done, **Reboot** your device or `launchctl reboot userspace` in NewTerm.

Now continue with normal delay OTA procedure: **[Restore RootFS](#heading)**.

Now remove the beta profile once you're finished.

# You're Done!

---

# Still need help?

---

Join the [r/Jailbreak](https://discord.gg/jb) Discord server.