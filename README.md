# Thinkpad-t480s-hackintosh-opencore

## Some folder in this repo:

```
- Sonoma-BCM94360NG: EFI for Sonoma ThinkPad T480s Card wifi BCM94352Z
    * FULL WORKING: Wifi, Bluetooth, Airdrop, Handoff, Sidecar...

- Sonoma: EFI for Sonoma ThinkPad T480s Card wifi Intel 8265

- Ventura: EFI for Ventura ThinkPad T480s Card wifi Intel 8265

 

```
## Result

About system:
![image1](./Images/image1.png)

Dual Screen:

![image2](./Images/image2.png)

Sidecar With ipad:

![image3](./Images/image3.png)


## Note
This repo base on:
https://github.com/Lost-Entrepreneur439/thinkpad-t480s-hackintosh

A prebuilt OpenCore EFI for macOS on the Lenovo ThinkPad T480s

**WARNING! If running Sonoma, ethernet IS required for initial half of setup if you use an internet-based installer. You will need to install Heliport for Wi-Fi. Ventura users can use Wi-Fi with no issues.**

Use 1.x releases for Ventura, 2.x releases for Sonoma.

This is a macOS EFI for the Lenovo ThinkPad T480s, with support for Intel Wi-Fi cards. Ventura and Sonoma compatible.

Follow the "Downloading macOS" section in the Dortania guide to get macOS. ***Support will not be offered if you get macOS from any other source.*** https://dortania.github.io/OpenCore-Install-Guide/installer-guide/windows-install.html#downloading-macos. After installing macOS, you will need to disable force clicking, as by default macOS will register all clicks as force clicks (System Settings -> Trackpad -> Uncheck "Force Click and haptic feedback")

## Specs of my specific unit
- CPU: Intel Core i7-8650U
- GPU: Intel UHD Graphics 620
- RAM: 24GB (8GB + 16GB)
- Touchpad: Elan SMBus
- Audio: Realtek ALC257
- Wi-Fi: Intel Wireless-AC 8265
- Ethernet: Intel I219-LM
- SSD: Samsung SSD 980 1TB
- Display: 14inch, 2k, IPS

## Set BIOS settings as follows
- Config -> Network -> Wake On LAN -> Disabled
- Config -> Network -> Wake On LAN from Dock -> Disabled
- Config -> CPU -> Intel (R) Hyper-Threading Technology -> Enabled
- Security -> Security Chip -> Security Chip -> Disabled
- Security -> Virtualization -> Intel (R) Virtualization Technology -> Enabled
- Security -> Virtualization -> Intel (R) VT-d Features -> Disabled
- Security -> Secure Boot -> Secure Boot -> Disabled
- Security -> Intel(R) SGX -> Intel (R) SGX Control -> Disabled
- Startup -> UEFI/Legacy Boot -> UEFI Only
- Startup -> CSM Support -> No

## Reference

https://github.com/Lost-Entrepreneur439/thinkpad-t480s-hackintosh

Thanks: Lost-Entrepreneur439, Van Hung Nguyen and Sang Nguyen

## Credits
- [Acidanthera](https://github.com/acidanthera) -- Made OpenCore, AppleALC, BlueToolFixup, BrightnessKeys, IntelMausi, Lilu, NVMeFix, SMCBatteryManager, SMCProcessor, SMCSuperIO, VirtualSMC, VoodooPS2Controller and WhateverGreen
- [OpenIntelWireless](https://github.com/OpenIntelWireless) -- Made Airportitlwm, IntelBluetoothFirmware and IntelBTPatcher
- [Avery Black](https://github.com/1Revenger1) -- Made ECEnabler
- [FireWolf](https://github.com/0xFireWolf) -- Made GenericCardReaderFriend
- [USBToolBox](https://github.com/USBToolBox) -- Made USBToolBox and UTBMap
- [VoodooSMBus](https://github.com/VoodooSMBus) -- Made VoodooSMBus
- [zhen-zen](https://github.com/zhen-zen) -- Made YogaSMC
- [CorpNewt](https://github.com/corpnewt) -- Made SSDTTime, which was used to make SSDTs.
- [dortania](https://github.com/dortania) -- Made the OpenCore Install Guide which was used to make this EFI.
- [Mohamed A. Salah](https://github.com/m4salah) -- Made another T480s EFI which I used a part from to fix mine not working.
- [ellnic](https://github.com/ellnic) -- Helped me fix Linux dualbooting