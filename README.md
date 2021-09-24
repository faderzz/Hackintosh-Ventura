
# Hackintosh with an AMD CPU and GPU 
**[WIP]**
 
 **This is not a guide** it is just a log on how I have managed to make this build and the issues I faced. 

**I have not booted into the USB as I have not finished this build yet** I do not know if I have built this correctly or not.


## Hackintosh Build Specs:

 - **Motherboard:** ASUS Prime B450+
 - **Graphics Card:** XFX RX 590 Fatboy
 - **CPU:** AMD Ryzen 7 2700x
 - **Storage:** 3TB Hitachi HDD
 - **Second Storage Device:** 256GB Corsair Force MP510 M.2 SSD

## Tools and Downloads
- [ProperTree](https://github.com/corpnewt/ProperTree) - To edit config.plist
- [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS) - To generate SMBIOS
- [Big Sur Guide](https://dortania.github.io/OpenCore-Install-Guide/extras/big-sur/#up-to-date-kexts-bootloader-and-config-plist) - Docs for Big Sur Installation with OpenCore
- [OpenCorePkg](https://github.com/acidanthera/OpenCorePkg/releases) - OpenCore
- [AMD Vanilla](https://github.com/AMD-OSX/AMD_Vanilla/) - Patches for AMD Hardware, read the repo for more info.

## SSDTs
Check the OpenCore guide as this is different for every CPU. Read the [OpenCore guide](https://dortania.github.io/OpenCore-Install-Guide/) for more info.

## Drivers
These should be the only drivers in **EFI > OC > DRIVERS**
- HFSPlus.efi
- OpenRuntime.efi

## Kexts
This is also depends on your hardware like SSDTs. Read the [OpenCore guide](https://dortania.github.io/OpenCore-Install-Guide/) for more info.
**My kexts are the following:**

- AppleALC
- AppleMCEReporterDisabler
- Lilu
- NVMeFix
- RealtekRTL8111
- VirtualSMC
- WhateverGreen

## config.plist
Read [the documentation for OpenCore](https://dortania.github.io/OpenCore-Install-Guide/) to make this properly.

**Note:** I did apply the [AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla/) patches

## Troubleshooting
I tried using GibMacOS to download MacOS Big Sur, format my USB, and install OpenCore but this did not work due to Big Sur images being built differently now. (Fuck you Apple 😭)

## 

**!!⚠ WARNING ⚠!!** This repo is for Educational Purposes only. I am not resposible for any damage done to your machine. 
