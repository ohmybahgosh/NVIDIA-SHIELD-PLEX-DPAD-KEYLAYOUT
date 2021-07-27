# NVIDIA-SHIELD-PLEX-DPAD-KEYLAYOUT
Keylayout fix that allows for pressing the dpad "OK" button to skip intro

## ROOT REQUIRED

## MAKE A DAMN BACKUP

### Info and What To Do:
So this keylayout is 99.9% stock, but I've replaced the mapping for the button Plex monitors when "skip intro" is pressed.  

.. I've simply remapped it to *"DPAD_CENTER"*. 

*Make a backup of /system/usr/keylayout/Generic.kl*

Copy the Generic.kl file from this repo, in to /system/usr/keylayout/Generic.kl

## *Command ONE-LINER (REQUIRES ROOT/ADB):*
```bash
git clone https://github.com/ohmybahgosh/NVIDIA-SHIELD-PLEX-DPAD-KEYLAYOUT.git && cd NVIDIA-SHIELD-PLEX-DPAD-KEYLAYOUT && adb shell mv /system/usr/keylayout/Generic.kl /system/usr/keylayout/Generic.kl.bak && adb push Generic.kl /system/usr/keylayout/Generic.kl && adb shell chmod 644 /system/usr/keylayout/Generic.kl
```

## AFTER REPLACING THE kl FILE, UNPLUG YOUR USB DONGLE FOR THE DPAD, THEN PLUG IT BACK IN. IF "SKIP INTRO", BY USING THE DPAD OK BUTTON STILL DOESN'T WORK, DO A REBOOT ON YOUR SHIELD! 
