# Pixel Experience
I made a compilation of the different mods and came up with this Pixel Experience module which can be flashed with other devices on Nougat.

## Information
As a Mi A1 user, I was stuck with Stock Oreo 8.0.0 without Oreo custom ROMs when I first bought my device. Kernel sources weren't released at the time so I decided if I can cook up a Magisk module that can bring me the Pixel Experience ROM without the need to install that certain ROM. What I did is to search around the internet which lead me to several mods on XDA, GitHub and other websites which have extracted files from the Pixel 2 devices. I've decided to gather them and compiled them all into a single Magisk Module. This module can be flashed with other devices on Nougat and above as well.

## Features
- Modded Pixel 2 Launcher by [@paphonb](https://forum.xda-developers.com/member.php?u=6018897) | [XDA thread](https://forum.xda-developers.com/android/apps-games/app-rootless-pixel-2-launcher-google-t3688393) | [Telegram channel for Launcher support](https://t.me/MPixelLauncher2)
- Rootless Pixel Launcher by [@azaidi](https://forum.xda-developers.com/member.php?u=3012129) | [XDA thread](https://forum.xda-developers.com/android/apps-games/launcher3-pixel-launcher-features-t3620972) | [Telegram channel for Launcher support](https://t.me/launcherthree)
- Ruthless (Pixel 2) Launcher by [@shubbyy](https://forum.xda-developers.com/member.php?u=6086799) | [XDA thread](https://forum.xda-developers.com/android/apps-games/app-ruthless-pixel-launcher-based-t3755903) | [Telegram channel for Launcher support](https://t.me/RPLauncher)
- Pixel accent (in system/vendor/overlay/Pixel)
- Google Lens enabled in Google Photos
- Google Sans font used in Google Assistant, Pixel Launcher, System Update window, SetupWizard text
- Pixel 2 audio (ringtones, notifications, ui, alarms)
- Enable Google Assistant via build.prop
- Camera2 API support (find a working Modded Google Camera app [here](https://www.celsoazevedo.com/files/android/google-camera/))
- EIS support
- Enables Night Light support (device/ROM dependent)

## Reminders
To avoid Launcher being renamed/crashing, disable the launcher you installed and switch to different launcher before disabling/uninstalling the module. Not doing so could result in a “0.0dip has stopped working" bug. If you do encounter this bug, try installing the real Pixel Launcher from the [Google Play store](https://play.google.com/store/apps/details?id=com.google.android.apps.nexuslauncher).

If you encounter bootloop when uninstalling the module, you need to flash the Rescue zip found [here](https://androidfilehost.com/?fid=673368273298925325) to disable all overlays. You should be able to reboot without any problems afterwards!

## Support
You may report any bugs via the new | [Telegram channel](https://t.me/PXMagisk)

## Latest changelog
v5.0
- Audio improvements for Xiaomi Mi A1 (use fluencepro and fix talkback for Google Assistant)
- Replace GoogleSans fonts from Android P Dev Preview 3
- Replace NotoColorEmoji with latest Emoji pack from Android P Dev Preview 3

v4.9
- Remove Google Unlimited photo storage (doesn't work; goes against Google Drive storage)
- Add a few more Pixel XML files
- Include framework files

v4.8
- Remove CPL from the module
- Added Amir's Launcher optimized for Android Go | [Telegram](https://t.me/appforks/821)

## Latest Launcher versions
- Modded Pixel 2 Launcher = 6 build 17 | [Telegram channel](https://t.me/getMpl)
- Rootless Pixel Launcher = 3.5 | [Telegram channel](https://t.me/appforks)
- Ruthless Pixel Launcher = 2.0 | [Telegram channel](https://t.me/ruthlaunch)

For old changelogs, check on the [XDA Thread](https://forum.xda-developers.com/showpost.php?p=75731833&postcount=2)

## STEPS TO ENABLE NIGHT LIGHT
You need to type this code via adb (connect your device to the PC with USB Debugging enabled)

adb shell cmd overlay enable --user 0 android.res.night

then reboot your device.

## Compatibility
- Asus Zenfone 2 Selfie, running RR 5.8.5 (Android 7.1.2)
- Cherry Mobile G1 on 8.1.0 LOS 15.1 (seed)
- HTC U11
- Huawei P10 with EMUI 8.0 (8.0.0.365) (c432) 
- Essential PH-1
- LeEco Pro 3
- LG G4 on AOSCP(CypherOS) 5.3(Android 8.1)
- LG G6 running RR 8.1
- OnePlus 3T
- OnePlus 5 on OOS Beta 5
- OnePlus 5 on 8.1.0 Omni ROM
- OnePlus 5T on OOS Beta 3
- OnePlus 5T on OOS 5.0.4
- Nexus 5
- Nexus 5x on 8.1.0
- Samsung Galaxy A5 (2017) LOS 15.1
- Samsung Galaxy Note 3 n9005 on 8.1 RR
- Samsung Galaxy S6
- Samsung Galaxy S8 Exynos - weather app crashes but no other issues found
- Sony Xperia Z2 on 8.1.0 Resurrection Remix Oreo
- Sony Xperia Z3 on Omni 8.1
- Sony Xperia XZ, SlimBit AOSP 8.1
- Wileyfox Swift on 8.1.0 crDroid (crackling)
- Xiaomi Redmi Note 4X (Mido) with MIUI 9.2.1 Global Stable
- Xiaomi Mi 5 Prime on 8.1.0 Omni ROM Oreo
- Xiaomi Mi 5X MIUI 9.2.2.0 Android 7.1
- Xiaomi Mi A1 on 8.0.0 Oreo Stock ROM (tissot)
- Xiaomi Mi A1 on Pixel Experience ROM 8.1.0
- Xiaomi Mi Max 2 running LOS 14.1
- Xiaomi Mi Mix 2
- Xiaomi Mi Note 2 with MIUI 9
- YU Yureka Black on AOSP Extended 7.1.2
- YU Yureka Black on Resurrection Remix 7.1.2
- Zuk Z2 Pro on Aex 5.2 Oreo
- Zuk Z2 Pro in Resurrection Remix v.6.0.0 and Aex 5.3

Provide feedback via the XDA thread by inputting your phone model, current ROM. Feel free to report if it works on other devices as well. It should work on other devices as long as they are close to stock (Stock/Custom ROMs).

## Thanks
Thanks to these people!
- @rprimus for helping out with the overlay.list issues to avoid system not booting issue in previous builds
- @tohtorin for helping out with the Unity script | [XDA profile](https://forum.xda-developers.com/member.php?u=7547198)
- @Zackptg5 for helping out with the Unity Installer | [XDA guide](https://forum.xda-developers.com/android/software/guide-volume-key-selection-flashable-zip-t3773410)
- @Rom for helping out the install.sh codes | [XDA profile](https://forum.xda-developers.com/member.php?u=5332893)
- @shubbyy for his Ruthless Pixel Launcher | [XDA thread](https://forum.xda-developers.com/android/apps-games/app-ruthless-pixel-launcher-based-t3755903/)
- @azaidi for his Rootless Pixel Launcher | [XDA thread](https://forum.xda-developers.com/android/apps-games/launcher3-pixel-launcher-features-t3620972)
- @paphonb for his Modded Pixel 2 Launcher | [XDA thread](https://forum.xda-developers.com/android/apps-games/app-rootless-pixel-2-launcher-google-t3688393)
- @Chronzy for providing the system/vendor/overlay files as well as system/media files from his Pixel 2. | [XDA thread](https://forum.xda-developers.com/showpost.php?p=74267243&postcount=14) 
- @elmkzgirxp for providing an overlay for the lockscreen font
- @Soheil_rf for his Night Light enabler overlay | [XDA thread](https://forum.xda-developers.com/crossdevice-dev/sony-themes-apps/oreo-enable-night-light-tile-t3713021)
- @topjohnwu for Magisk

LICENSE
Copyright © 2018 joeyhuab. Licensed under the GNU General Public License v3.

## [XDA Portal feature](https://www.xda-developers.com/pixel-2-experience-magisk-module/)
## [XDA Official thread](https://forum.xda-developers.com/apps/magisk/module-pixel-2-experience-t3757137/)
## [Github source](https://github.com/joeyhuab/Pixel-2-Experience-Magisk/)
