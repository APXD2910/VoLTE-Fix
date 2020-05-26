# VoLTE-Fix
Fixes Qualcomm VoLTE on all GSI Treble Roms

> ### Note: All scripts to be run via adb on a computer

# Usage
## Using install.sh
> Note: If you're not rooted, boot into TWRP, and mount system as r/w. Also keep in mind that some recoveries mount system as /system_root instead of /system. In that case, use install-system_root.sh

Run

``./install.sh 32`` if you're on a arm device

``./install.sh 64`` if you're on a a64 or arm64 device

## Manually
### For a64 or arm64
Copy the binder64/ims (don't copy the binder64 folder, only the ims folder inside it) folder to /system/priv-app and copy android.hardware.telephony.ims.xml to /system/etc/permissions

### For arm
Copy the binder32/ims (don't copy the binder32 folder, only the ims folder inside it) folder to /system/priv-app and copy android.hardware.telephony.ims.xml to /system/etc/permissions

# For dummies

- [What is adb?](https://www.xda-developers.com/what-is-adb/)
- Where should I download adb and fastboot without downloading the entire android sdk? Downloads: [Windows](https://dl.google.com/android/repository/platform-tools-latest-windows.zip), [macOS](https://dl.google.com/android/repository/platform-tools-latest-darwin.zip), [Linux](https://dl.google.com/android/repository/platform-tools-latest-linux.zip) (These links are maintained by google, you should always get the latest versions)
- How do I download this repository? Use the download button above or just click [here](https://github.com/KhushrajRathod/VoLTE-Fix/archive/master.zip).
- How do I install the apks? You need to run install.sh. See how to run a shell script on [windows](https://www.thewindowsclub.com/how-to-run-sh-or-shell-script-file-in-windows-10), [macOS/Linux](https://askubuntu.com/a/38670) 
