# Jflte DevCon Team
### Developers & Testers
[B--B](https://github.com/B--B) - Lead

[AntaresOne](http://github.com/AntaresOne) - Developer, git mantainer, scripting, tester

[Alucard24](http://github.com/Alucard24) - Kernel Developer

[MatthewBooth](http://github.com/MatthewBooth) - OTA Updates, git maintainer, scripting, tester

[angelcalibur](https://github.com/angelcalibur) - Tester

[smeroni68](https://github.com/smeroni68) - Tester

[Jimsilver73](https://github.com/Jimsilver73) - Tester

[hawkerpaul](https://github.com/hawkerpaul) - Tester, scripting

[franzyroy](https://github.com/franzyroy) - Tester, cm themer

[smstiv](https://github.com/smstiv) - Tester

[side](https://github.com/dkati) - Tester, cm themer, rom maintainer

[javelinanddart](https://github.com/javelinanddart) - Kernel Developer

[srisurya95](https://github.com/srisurya95) - Rom-Kernel Developer

[gadget!](http://forum.xda-developers.com/member.php?u=2026779) - Themer, tester, graphic designer

[MZO9400](https://github.com/MZO9400) - Developer, git mantainer, scripting, tester, OnePlus 2 Mantainer

### Changelog (full)
[AOSP-JF-MM](https://github.com/AOSP-JF-MM) - Project GitHub

### Changelog (short)

#### Ongoing changes (Stable 6)...
* Kernel (OnePlus2)
    * Linux 3.10.105
    * Disable SDCardFS for now
    * Switch to Google Nexus 6P's optimized interactive governor
* Kernel (Gemini)
    * General code updates
    * Small enhancements for EAS
    * Ramdisk: move to schedutil governor
    * Ramdisk: port fs tune settings from Marlin
    * Ramdisk: relax top-app boost
    * Ramdisk: configure cpuset at boot complete
* ROM
    * OnePlus2: Speed up Fingerprint sensor's response
    * build/kati: Suppress FindEmulator spam
    * OnePlus2: Use HAL3 Camera
    * frameworks/av: Use HAL3 patches for OnePlus2
    * system/sepolicy: Use HAL3 patches for OnePlus2
    * device/qcom/sepolicy: Use HAL3 patches for OnePlus2
    * Gemini: fixed slomo recording with Google Camera
    * Gemini: enable 32 bit specific optimisations for kryo
    * system/core/rootdir: fix cpuset not set properly sometimes after the boot
    * General translation updates
    * vendor/aosp: fixed some props not set properly in build.prop

#### Stable 5.1 (20170424)
* Kernel (OnePlus2)
    * Merge OOS 3.5.8 changes
    * Merge latest SDCARDFS
* Kernel (Gemini)
    * Fixed QC3
* ROM
    * Camera: fix audio recording when taking video
    * Updated translations
    * OMS: ThemeInterfacer: ported TeamSubstratum binder changes (pending on gerrit)
    * Vendor/OnePlus2: merge in latest OOS blobs

#### Stable 5 (20170423)
* Kernel (Gemini)
    * Added and enabled KCAL support
    * Sdcardfs: general code updates/fixes
    * General updates/fixes for EAS
    * General code update
    * Ported google binder changes from msm-3.18 kernel O preview
    * SafetyNet check: pass CTS tests in a better way
    * Removed unused LiveDisplay driver
    * Set WALT as default
    * Disable crc check
    * Fixed sdcardfs (was the cause of random shutdown)
    * Merged CAF tag LA.UM.5.5.r1-04300-8x96.0
* Kernel (jflte)
    * SafetyNet check: pass CTS tests in a better way
    * Ramdisk: fixed some scripts not working with Magisk
* ROM
    * packages/apps/CellBroadcastReceiver: Merged 7.1.2 sources over CAF branch
    * system/bt: merged Android 7.1.2 Release 4 changes
    * services/Telephony: various fixes
    * OTAUpdates: fixed ROM and addons download (again)
    * SnapdragonCamera: general updates/fixes
    * PowerManager: Bring back the compatibility with AOSP
    * Auto brightness: fix weird brightness jumps (especially in low light conditions)
    * packages/apps/Nfc: port missing changes from Android 7.1.2 r4 release
    * Fixed browser compiling and added back to build
    * OMS: updates from latest gerrit chages
    * Substratum: update to v672
    * Updated JDCTeam bootanimation vs Pixel style (Thanks to @gadget!)
    * fb/base: general fixes from upstream
    * Settings: import ES HR NL RU PL FR translations for our custom settings
    * General translations updates
    * system/bt - SnapdragonCamera: merged CAF tag LA.UM.5.5.r1-04300-8x96.0
    * msm8996 HALs: merged CAF tag LA.UM.5.5.r1-04300-8x96.0
    * media: implement radio_metadata wrapper for safer memory management
    * fw/av: general fixes from upstream
    * jf: update Time Service blobs
    * jf: fix auto time zone not working for some variants

#### Stable 4 (20170408)
* Kernel (Gemini)
    * Bypass SafetyNet check
    * EAS: sync with Marlin code
    * EAS: update to v1.2 from Google
    * Update kernel sources and qcacld-2.0 to caf tag LA.UM.5.5.r1-04000-8x96.0
    * Fixed CVE-2017-0583
    * General code updates/fixes
    * Merged CAF tag LA.UM.5.5.r1-04000-8x96.0
* Kernel (JFLTE)
    * Bypass SafetyNet check
    * Updated ramdisk scripts for Magisk root
    * Fixed CVE-2017-0583
* Kernel (OnePlus2)
    * Fixed CVE-2017-5967
* ROM
    * Gemini: fixed D2TW feature (feature was missing in Marlin power HAL)
    * Settings: fix settings crash when user opens Storage Manager
    * Updated translations
    * Gemini: Ramdisk: add init.power.sh to manage EAS and other PM
    * Gemini: Ramdisk: clean power config and add EAS'd perfd
    * Gemini: improved battery life 
    * DeskClock: various fixes
    * SuperUser: drop SuperSU in favour of Magisk and MagiskManager
    * Settings: fixed expanded desktop menu
    * Add back AOSP Exchange services
    * Jflte: Provide a working version of Toolbox with Magisk
    * init.rc: add back CAF schedtune changes, EAS 1.2 supports 5 groups
    * frameworks/base: added our battery customisations
    * NavBar: ported Pixel NavBar + fixes (REVERTED, must be updated for 7.1.2)
    * Jflte: HAX: fix tethering (thanks to @rothmark (xda))
    * OMS: sync with TeamSubstratum gerrit
    * OMS: Hold "volume up" during boot to disable all overlays
    * Bluetooth: Fix setting app stoped when unpair device
    * LatinIME: various updates and fixes
    * LatinIME: added more languages and dictionaries
    * BackupTools: various updates
    * Rebased build repo, fixed some weird log errors in TWRP during ROM flashing
    * Update sources to Android 7.1.2 Release 4 (N2G47H)
    * Updated and fixed CAF code after AOSP change
    * JDC Custom settings: update italian translations
    * Substratum: update to v631

#### Stable 3 (20170328)
* Kernel (JFLTE)
    * General code updates
    * net: general fixes/updates
    * Fixed sporadic screen flickering issue
    * Battery: fixed wrong battery calculation
* Kernel (Gemini)
    * Merged CAF tag LA.UM.5.5.r1-03800-8x96.0
    * Updated sources to latest linux release (3.18.48)
    * Fixed various memory leaks
    * Fixed wifi disconnection issues
    * Ported and enabled EAS and all related features (sched, walt, cgroups, cpusets, memcg and a lot of other things)
      Big thanks to RenderBroken and Alucard24 for their huge work
    * Ported Alucard24 alucard_sched governor (WIP) and EAS energy model optimisations specific for QCOM 8996AB
    * General code updates/fixes from LOS
* Kernel (OnePlus2)
    * Initial Release
* ROM
    * oppo/common: OnePlus2: Fix OOS Gestures and Tri-State Key
    * frameworks/base: various fixes from upstream
    * system/core: small fixes on init.rc and libcutils
    * Add night display feature for all devices
    * Added missing charging images for charging when phone is powered off
    * Updated translations
    * Updated msm8996 HALs to CAF tag LA.UM.5.5.r1-03800-8x96.0
    * SnapdragonCamera: merged CAF tag LA.UM.5.5.r1-03800-8x96.0
    * Gemini: rootdir cleaning, removed tons of unuseful stuffs
    * Gemini: updated device tree for EAS support
    * Gemini: enabled CPUSETS and EAS enhancements
    * Gemini: use Marlin power HAL and perfd blobs with full EAS support
    * Gemini: fixed SnapdragonCamera with HAL3 enabled
    * Gemini: updated audio conf
    * Gemini: turn off carrier provisioning and allow tethering for everyone
    * Added allow unlinking ringer with notification volume feature
    * OMS: merged all latest official updates
    * init.rc: removed CAF code that breaks EAS/schedtune --> back to AOSP
    * Gemini: ramdisk/blobs: another big cleaning of unseful stuffs
    * jflte: SnapdragonCamera: fixed panorama mode
    * Added OnePlus 2 to buildable (and official supported) devices, big big thanks to MZO!
    * system/bt: merged CAF tag LA.UM.5.5.r1-03800-8x96.0

#### Stable 2 (20170312)
* Kernel (JFLTE)
    * General code updates
    * f2fs: update driver to 3.18.y
    * exFAT: update, fix and enable kernel driver
    * sdcardfs: general bug fixes
    * Ported binder changes from dorimanx kernel
    * Fixed f2fs issues with SuperSU
    * Disable CPUSET code and allow kernel to dist CPU PWR
    * Update TC to Linaro GCC 6.3.0
* Kernel (Gemini)
    * Rebased from LA.UM.5.5.r1-02500-8x96.0 revision
    * Fixed f2fs issues with SuperSU
    * Fixed QC3
* ROM
    * Update sources to Android 7.1.1 release 26
    * JFLTE: exfat: use kernel driver
    * SuperSU: update to v2.79 SR3
    * Substratum: update to v604
    * JFLTE: update webview to v57.0.2987.54 Beta
    * Updated ROM TC with latest Linaro patches
    * APNs updates
    * Rebased all repos with latest CAF N-MR1 branches
    * Base: added One-Hand mode UI (compatible with HW buttons)
    * Settings: add HW buttons light controls
    * Fixed a weird random bug that sometimes keep HW buttons light on when the screen is off (and kill deep sleep)
    * JFLTE: fixed camera
    * JFLTE: fixed reboot
    * Settings: fixed USB Tethering
    * OMS/Substratum: move to rootless
    * OMS: Expose more colors
    * JFLTE: Bluetooth: disable absolute volume
    * HW buttons customisations: added more functions (split screen and one hand UI)
    * Settings: Developer Options: OMS: add an option for allow theme app from unknown sources
    * Settings: Developer Options: added an option for kill app with long-press of back button
    * Cleaned tons of unused/unwanted CAF changes
    * Gemini: added "swap buttons" function
    * Gemini: added "use fingerprint as home button" feature
    * Gemini: update graphics blobs from revision LA.UM.5.5.r1-02500-8x96.0
    * msm8996: audio/media/display: rebased from CAF revision LA.UM.5.5.r1-02500-8x96.0
    * Gemini: Camera: enable HAL3 (fixes video recording issues and Google Camera)
    * JFLTE: update graphics blobs from flo mob30x
    * Toolbox: fixed for systemless root
    * A lot of things that i don't remember

#### Stable 1 (20161212)
* JFLTE
    * Back to v1.5 (Fixes freeze when screen is off experienced in some variants)
* Gemini
    * General code updates
    * Disabled Cpusets
* ROM
    * Fixed a NPE in setup wizard
    * Settings: Enable storage manager like Pixel devices
    * base: tuner: enable navbar config + added more icons
    * webview_packages: prefer the more powerful webview package installed
    * Gemini: build power HAL
    * Gemini: fixed dt2w feature
    * jflte: move to common consumer IR HAL
    * Add lg G5 (h850) to buildable devices
    * OMS: expose some hardcoded colors
    * Updated translations
    * Settings: drop JDCSettings and move all our custom features into settings
    * SystemUI: Enable three icon switching within QS DND tile
    * Status bar: added HSPA+ icons
    * Pixel Theme Framework Edits
    * Fixed reboot in recovery dialog title
    * Added screen record shortcut (Vol+ and power button)
    * Settings: fingerpint: allow devices to configure sensor location
    * Settings: expose PhoneInfo
    * OTAUpdates: updated and fixed for N 
    * Gemini: fixed video recording
    * OMS: merged all latest changes from TeamSubstratum
    * Gemini: fixed data/wifi switch issue
    * Gemini: disable Cpusets
    * Gemini: general blobs and conf updates from stock N
    * frameworks/base: port some UPSTREAM fixes
    * General APNs updates
    * Sepolicy: general updates from CAF
    * Gemini/jflte: remove no more needed Overlays
    * Jflte: liblights/consumerir: drop device level HAL and move to common HAL
    * Update sources to Android 7.1.1 release 4
    * Gemini: fix H+ icon (Workaround)
    * Camera2: allow to use power button as shutter
    * vendor/aosp: overlays: fixes + updates
    * Settings: enable gesture manager
    * frameworks/base: fixed GApps perms

#### Beta 2 (20161126)
* Kernel (Gemini)
    * General code updates and fixed boot on N
* Kernel (JFLTE)
    * General code updates
    * Kernel Patch 3.4.112->113 (only missing/good parts)
* ROM
    * JDCSettings: added custom hw key rebindings feature
    * JDCSettings: added long press volume button skip tracks feature
    * Fixed device storage menu when using Adopted Storage
    * Fixed an NPE when ejecting the portable storage
    * Don't dex preopt prebuilt APKs
    * Gemini: update blobs from Oneplus 3 repo
    * Gemini: more fixes/updates for N
    * Gemini: move to QCOM shared graphics driver repository
    * jflte: bluetooth: fixed  a crash caused by alarmtimer --> NOTE: this will break BT on stock kernel
    * jflte: update Widevine libraries
    * jflte: move to common graphics blobs repo
    * Update APNs
    * GCC: move to Linaro 4.9 Toolchains
    * Updated translations
    * Gemini: fixed perf issues when battery level is under 5%
    * JDCSettings: Added power menu customisations
    * Added ScreenRecord feature --> available in power menu
    * jflte: enable sdcardfs
    * jflte: VZW: fixed mobile data reconnection and IMSI issues, hopefully fixed for Sprint variant too
    * SuperSU: update to v2.78 SR4
    * Substratum: update to v490
    * WIP: added Expanded Desktop feature
    * Airplane mode toggle: small fixes/enhancements
    * frameworks/base: removed unused videos/drawables/media tests
    * Don't refresh ui when screen off
    * jflte: init.qcom.rc: update ril-service daemon

#### Beta 1 (20161118)
* Kernel (JFLTE)
    * Compile with GCC 6.0.1 + fixed compiling warns
    * General code updates
    * VoIP: more fixes + updates
    * Fixed sdcardfs
* ROM
    * WIP: initial Xiaomi Gemini bringup
    * Ported + fixed all CAF code on our repos
    * Deskclock: temporary revert CAF additions until bootloop issues are fixed
    * Bluetooth: fix JFLTE bluetooth after CAF code merge
    * WIP: bring back browser from MM
    * Gallery2: switch to SnapdragonGallery + cm fixes/enhancements
    * jflte: Add support for Samsung extended AGPS
    * STweaks: fixed profile check
    * Fix SuperSU installation for block-based OTAs
    * SuperSU: update to v2.78SR1
    * Substratum: update to v470 (is needed a full uninstall/removing of installed themes and overlays!)
    * jflte: GPS: removed not used files/services
    * msm8960: audio: fixes for voip and calls
    * msm8960: display: fixes and improved portability
    * jflte: remove some QC encoders from codecs list
    * Update sources to Android 7.1.0 release 7
    * Dialer: add back call recording feature
    * WebWiev: update to latest stable and beta versions released by Google
    * jflte: remove unused graphics libraries
    * jflte: more fixes for VoIP mixers
    * Jflte: init: fixed boot and network for all variants
    * OMS: Reverted all old patches and merge updated code from TeamSubstratum gerrit
    * jflte: updated sepolicies
    * APNs updates
    * jflte: libwvm.so: fix library crash due to missing symbol
    * Bootanimation: updated for 7.1. Big big thanks to @gadget! (xda)
    * Create 0 compression ratio jar files
    * telephony: Hack GSM and LTE signal strength
    * jflte: QMUXD: fixed acquire/release wakelocks
    * core: arm: remove deprecated -msoft-float in favour of -mfloat-abi=softfp
    * Xposed: jni: consider /data/app to the fd whitelist if Xposed is detected

#### Alpha 2 (20160902)
* Kernel
    * Fixed boot on N
    * Ramdisk: updated and fixed scripts for N
    * Ramdisk: updated and fixed scripts for systemless root
    * Merged latest 3.18 fixes/updates for ext4
    * General code updates/fixes
    * Fixed CVE-2015-8839
* ROM
    * Added exfat and NTFS support
    * System Sounds: use Stereophonic & Remastered Nexus sounds
    * Materialized some old icons/colours/toasts
    * Fixed NFC
    * Speed up animations
    * Audio: enabled custom audio policy again
    * Sepolicy: fixes + partial updates for N
    * frameworks/native: ported CAF code (mostly on surfaceflinger)
    * Add back changelog to Settings
    * SystemUpdateService: enable service but lock its receivers
    * Frameworks/base: general optimisations
    * skia: ported CAF code
    * Camera: various fixes
    * Build: fixed backuptools and override props functions
    * Build: completely reworked ROM versioning
    * OMS: exposed almost all harcoded colours (WIP)
    * native: ported cm fixes for QCOM devices
    * Webview: use Google WebView version instead of stock AOSP
    * Fixed LEDify
    * STweaks: fixed systemless root detection
    * SuperSU: update to v2.78
    * Settings: general fixes/enhancements and some icon materialization
    * Base: partially ported CAF code/optimisations
    * Update sources to Android 7.0.0 release 6
    * RIL: removed old LP hack for NO SIM issue in Airplane Mode and fix things in a proper way

#### Alpha 1 (20160901)

* Initial public release
