+++
title = "Delay OTA - un-Jailbroken"
date = "2022-01-14T17:58:40-05:00"
author = "flower"
authorTwitter = "" #do not include @
cover = ""
tags = ["delayota", "NotJailbroken"]
keywords = ["delayota", "NotJailbroken"]
description = "You can update using DelayOTA to versions for up to 90 days after a new version is released."
showFullContent = false
readingTime = false
+++

![del](del.png)

You can update using DelayOTA to versions for up to 90 days after a new version is released.
- *This will **NOT** need any sort of Blob, it acts like a normal OTA update you'd see in settings.*

Thank you **[DhinakG](https://github.com/dhinakg/)** for discovering this awesome method!

**HUGE** thank you to **[Saunders Tech](https://www.youtube.com/c/SaundersTech)** for making this [video](https://www.youtube.com/watch?v=vKgI55PL-ag&t) and for providing the backup used in this guide!

# Requirements

---

Previously made backup.

Personal Computer
- *Either running `Mac` or `Windows`, **Linux** users can't use this method unfortunately.*

- *Any work or school computer may **NOT** work, these methods need Admin Permissions to function.*

iOS 11+
- *If you're not sure on what iOS version you're currently on go to:*

`Settings` -> `General` -> `About` *and look at `Software Version`.*

If you have a Jailbroken device go **[here]()**.
- *You can **keep** data if you use this method linked.*

[iBackupBot](https://www.icopybot.com/ibackupbot_setup.exe) `Windows`

- *You will also need [iTunes](https://www.apple.com/itunes/download/win64).*

[Apple Configurator 2](https://apps.apple.com/us/app/apple-configurator-2/id1037126344?mt=12) `Mac`


# For un-Jailbroken devices `Hardest`

---

If you have `Windows`, go **[here](#windows---using-ibackupbot-free)**.

If you instead have a `Mac`, go **[here](#mac---using-apple-configurator-2-free)**.

Once done, move on to **[Installing the profile](#installing-the-profile)**.

# Windows - Using iBackupBot `Free`

---

Download `ibackupbot_setup.exe` from the requirements section and set it up like normal.

- *Make sure you have [iTunes](https://www.apple.com/itunes/download/win64) as well.*

> Note that this method will **LIKELY** erase all your data, make sure you make a backup of the device before proceeding.

Once set up, make sure you have plugged in your device and trusted it.

- *If you're having trouble having iBackupBot detect your device please reinstall iTunes, and check if your cable is working currectly.*

Now, if all goes well your device should popup in iBackupBot.

Download the pre-made backup **[here](https://cdn.discordapp.com/attachments/836793351818706984/932382833782165504/Supervision.zip)**.

Extract the zip, and open it. You'll see a folder called `Supervision`.

> If you haven't figured it out already, you'll be using a pre-made backup so you can get your device supervised.

Open `iBackupBot`.

![ibackupbot](ibackupbot.png) 

Go press the folder icon in iBackupBot , and select the `Supervision` backup.

- *Or do `CTRL + O` and select it.*

Now iBackupBot should display the Backup you've selected.

![ibackupbotselect](ibackupselect1.png)

Go into the backup, and press on `System Files`.

![ibackupbotselect](ibackupconfig.png)

Once you selected the folder, now search for `config`.

![ibackupbotselect](ibackupprofiles.png)

Now, select `ConfigurationProfiles` and press `Restore`.

![ibackupbotselect](ibackuppasswd.png)

It will ask you for a password, the password is `1234`.

Press `OK`.

Now, your device will begin restoring the the provided backup.

- *This should take around a 1 - 3 minutes, it's fairly quick.*

Check Settings, if it says `This device is supervised and managed by stkc.win.` Then you did correctly!

You can now move on to **[Installing the profile](#installing-the-profile)**.

# Mac - Using Apple Configurator 2 `Free`

---

Download `Apple Configurator 2` from the requirements section and set it up like normal.

> Note that this method **WILL** erase all your data, make sure you make a backup of the device before proceeding.

Once set up, make sure you have plugged in your device and trusted it.

![ac2](ac2.png) 

Press on your device, and press `Prepare` and select `Manual supervision`.

- *Also make sure you have `Supervise devices` toggled.*

Next, choose `Do not enroll in MDM`.

Then go to `Organization`, and click `New Organization`.

Either sign in to your `Apple ID`, or click `Skip`.

- *It's recommended to just `Skip` it.*

- *If you chose to skip signing into your Apple ID, add a name, then click `Next`.*

Choose `Generate a new supervision identity`.

- *If you've done this before in Apple Configurator 2, you can Choose an existing supervision identity instead.*

Configure the `iOS Setup Assistant` as you wish.

- *If you forgot to backup your data earlier in the guide, this is the last step where you'll be able to do this.*

Click `Prepare`, which will erase your device and supervise it.

Check Settings, if it says `This device is supervised and managed.` Then you did correctly!

# Installing the profile

---

If you're supervised to should do the following:

Install the profile you want DelayOTA to **[here](https://dhinakg.github.io/delayed-otas.html)**.

- *If you have an iPhone `12` or `13`, please use the `iOS (iPhone 12 series/13 series only)` section.*

- *If you have an iPhone `11` or **older** device, please use the `iOS (all other non-legacy devices)` section.*

- *This website will show the current available versions right away.*

Then, go to settings and search for the profile, go to:

`Settings` -> `General` -> `Profiles & Device Management`

Press on **install** when you select the profile, right after `Reboot` your device.

- *If it shows that it's `Not Signed` ignore it.*

Go into Settings and see if the update is there:

`Settings` -> `General` -> `Software Update`

- *If the update is has an **error** or it says that it's **Up to Date**, please install `OTAEnabler` in your package manager*.

- *If you're using **unc0ver**, please **[Restore RootFS]()** a second time but with `Automatic Software Updates` enabled*.

Press `Download and Install`.

> Make sure you use your backup after the install!

# You're Done!

---

# Still need help?

---

Join the [r/Jailbreak](https://discord.gg/jb) Discord server.







