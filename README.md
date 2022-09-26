
# MDMPatcher Universal

## Compability

- *should* work on iOS 15+
- *should* work on 64bit devices up to iPhone 13

## System requirements
macOS 10.13 or higher, Intel or M1.


## Helpful for u?
BTC > bc1qvcq852yggaxj0pls9u58f9lc9kc6hk0vg8uc49

## Credits
Nikias Bassen & rest of libimobiledevice team
(for idevicebackup2)

...and other people which i may forgot, I'm sorry...

9/26/22
Instructions for Mac. (My setup was a MacBook Pro M1 bypassing MDM on an iPad Air 2 Cellular):

1. visit https://ipsw.me/ and download the ipsw file for your iOS device.
    - to know which ipsw to download, lookup the model number on the back of your iOS device, e.g. A1567. Then, match the generation name to the model number on a site like https://www.theiphonewiki.com/wiki/Models. For example, A1567 is iPad Air 2. Once you know the name of the iOS device you have, you can download the appropriate IPSW. If you can't decide between the cellular version of the ipsw and the wifi only version, check the outer casing of your iOS device. For example, if you have an iPad and there is a slot for a SIM card on the body of the iPad, then you have a cellular device; download the cellular IPSW.

2. Put your iOS device into Recovery Mode while connected to the computer you just downloaded the IPSW file to. For help on entering this mode, visit:
    - https://support.apple.com/en-us/HT201263
    - https://support.apple.com/en-us/HT212787
    (For my iPad Air 2, the process was simply holding the power button and the home buttons until a message displayed on the iPad screen to connect it to the computer.)

3. Once your iOS device has entered recovery mode, from your computer, a message should ask if you want to update or restore your device. Hold the OPTION key on your computer and click to UPDATE or RESTORE your device.

4. From the popup window, find and select the IPSW file you just downloaded, then click OPEN. Select UPDATE or RESTORE and wait for the software to be extracted and installed.

* If the process fails to install, try again making sure you don't have the MDMUniversal Patch app open.
** If all else fails, you may try the Update or Restore process without installing the downloaded IPSW file. (I did not do this.)

Once the install process has completed, your iOS device should reboot.

5. Follow the instructions on the iOS device which should begin by choosing a language, then a Country or Region. Stop when you get to the screen to choose your wifi network.

6. While your iOS device is connected to your computer, open the MDMPatcher app. 
    - if it fails to open, right-click the app to open, then choose OPEN.
    - if right-clicking fails to open, you'll need to disable SIP on your computer.
    How to disable SIP on an M1 MacBook Pro.
    1. Shut down your computer.
    2. Hold the power button until the computer turns on and tells you that it's loading options.
    3. Choose Options and not your Hard Disk Drive.
    4. From the top menu, choose to open the terminal.
    5. Enter the command csrutil disable
    6. Restart your computer.
    7. Open the MDMPatcher Universal App.
7. On your Mac, open Finder. Click your iOS device that you're trying to use the MDM Bypass on. The screen may say something about "Activating...". If it does, wait until this screen says to "Get Started".
8. Make sure your device information is displayed on the MDMPatcher window instead of --- --- ---. If it is not, quit the MDMPatcher App and re-open it. Once your iOS device information is displayed, click PATCH.
9. Your iOS device will reboot and say that it has been restored.
10. Follow the rest of the setup instructions on your iOS device, including connecting to wifi. It should be done.