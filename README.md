[![macOS version](https://img.shields.io/badge/macOS-11.5.2%20(17G14042)-informational.svg)](https://www.apple.com/macos) [![OpenCore version](https://img.shields.io/badge/OpenCore-0.7.2-informational.svg)](https://github.com/acidanthera/OpenCorePkg) 

# AMD-Ryzentosh Ryzen 9 5900x Gigabyte B550M Auros Pro RX 6800

OpenCore 0.7.2 configuration for Amd zen 3 and Rx 6800. You must add your own serial number, MB serial, and uuid for imessage to work. To fix kernel panics when entering sleep mode disable wake for ethernet. When installing, disable CSM in bios as well as XMP.


## Hardware

| Type                 | Name                              |
|----------------------|-----------------------------------|
| CPU                  | AMD Ryzen 9 5900x                 |
| MB                   | Gigabyte B550M Auros Pro.         |
| Audio                | Realtek                           |
| GPU                  | Red Dragon Radeon AMD RX 6800     |
| RAM                  | 32G 3600Mhz DDR4 (16G * 2)        |
| Ethernet             | Realtek Gigabit Gaming Network    |
| Disk                 | Samsung 970 Pro 1TB               |



![ScreenShot](<iframe src="https://drive.google.com/file/d/1vBpl4dmm988U0CJyb49S-0bD8hymcyAC/preview" width="640" height="480" allow="autoplay"></iframe>)

## ACPI
- [SSDT] SSDT-CPUR.aml
- [SSDT] SSDT-EC-USBX-DESKTOP.aml

## Patches & Kexts
 - [[Patch] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
 - [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
 - [[Kext] Lilu](https://github.com/acidanthera/Lilu)
 - [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
 - [Kext] AppleMCEReporterDisabler
 - [Kext] AMDRyzenCPUPowerManagement
 - [Kext] RealtekRTL8111
 - [Kext] USBInjectAll.kext



## What's working:

* Ethernet (Realtek Gigabit Gaming Network Connection)
* Display Port audio (though no volume control)
* Audio output
* Sleep
* iCloud, iMessage, Facetime
* Front USB ports are working
* Back USB ports are working
* Graphics
* FileVault
* Docker
* Adobe Products (Photoshop, XD)

## What's not working:
* Microphone input 
* Hardware Virtualization (VirtualBox is working fine, but Parallels isn't)
