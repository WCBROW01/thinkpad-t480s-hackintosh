# thinkpad-t480s-hackintosh

A prebuilt OpenCore EFI for macOS on the Lenovo ThinkPad T480s, based on the work of [Lost-Entrepreneur439](https://github.com/Lost-Entrepreneur439).

This is a macOS EFI for the Lenovo ThinkPad T480s, with support for Intel Wi-Fi cards. Currently, Ventura and Sonoma are supported. Sequoia should work with minimal changes, but this laptop is my daily driver, so anybody who wants a Sequoia-compatible EFI will have to wait until I get around to running it.

Follow the ["Downloading macOS" section in the Dortania guide](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/) to get macOS. ***Support will not be offered if you get macOS from any other source.*** After installing macOS, you will need to disable force clicking, as by default macOS will register all clicks as force clicks (System Settings -> Trackpad -> Uncheck "Force Click and haptic feedback")

![Screenshot](https://github.com/WCBROW01/thinkpad-t480s-hackintosh/blob/main/untitled.png)

# Specs of my specific unit:
- CPU: Intel Core i5-8350U
- GPU: Intel UHD Graphics 620
- RAM: 24GB (8GB soldered, 16GB Samsung stick inserted)
- Touchpad: Elan SMBus
- Audio: Realtek ALC257
- Wi-Fi: Intel Wireless-AC 8265
- Ethernet: Intel I219-LM
- SSD: Intel 660p 512GB

# Set BIOS settings as follows
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

# Credits
- [Lost-Entrepreneur439](https://github.com/Lost-Entrepreneur439) -- Made the EFI this was based on
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
