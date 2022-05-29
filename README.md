# AMD Ryzen Hackintosh - Opencore EFI for Asus Prime B450M-II


## Specification
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 3 1200 @ 3.1GHz |
| Motherboard |  Asus B450M-II Prime |
| RAM | 16GB (2 x 8GB) Kingston Fuzy @ 3200MHz |
| Audio Chipset | Realtek® ALC892/ALC897 Codec |
| GPU | Gigabyte AMD RX460 |
| Ethernet | Realtek® RTL8111H |
| WiFi | TL-WN823N |
| Bluetooth | TPLink UB400 |
| OS Disk (NVME) | Kingston NV1(MVME) 256GB  |

**macOS version**: 11.4   

**OpenCore version**: 0.7.2

**SMBIOS**:  MacPro7,1

![](1.png)

## Drivers & Kexts
 - [[Bootloader] OpenCore](https://github.com/acidanthera/OpenCorePkg)
 - [[Patch] AMD_Vanilla](https://github.com/AMD-OSX/AMD_Vanilla)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
 - [[Driver] OpenRunTime](https://github.com/acidanthera/OpenCorePkg)
 - [[Driver] HfsPlus](https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi)
 - [[Driver] OpenCanopy](https://dortania.github.io/OpenCore-Post-Install/cosmetic/gui.html)
 - [[Kext] Lilu](https://github.com/acidanthera/Lilu)
 - [[Kext] VirtualSMC](https://github.com/acidanthera/VirtualSMC)
 - [[Kext] WhateverGreen](https://github.com/acidanthera/WhateverGreen)
 - [[Kext] AppleALC](https://github.com/acidanthera/AppleALC)
 - [[Kext] AppleMCEReporterDisabler](https://github.com/AMD-OSX/AMD_Vanilla/blob/opencore/Extra/AppleMCEReporterDisabler.kext.zip)
 - [[Kext] RealtekRTL8111](https://github.com/Mieze/RTL8111_driver_for_OS_X)
 - [[Kext] NullEthernet](https://github.com/RehabMan/OS-X-Null-Ethernet)
 - [[Kext] AMDRyzenCPUPowerManagement](https://github.com/trulyspinach/SMCAMDProcessor)
 - [[Kext] SMCAMDProcessor](https://github.com/trulyspinach/SMCAMDProcessor)


## Working
- Xcode
- iMessage
- Android simulator
- FaceTime
- Sleep & Wake
	
- Wireless
- Bluetooth
- Audio
- DRM 
- USB
- Etc.


## How to use
  1. Create directory "EFI" in your EFI partition (e.g. pendrive or hard drive)
  2. Clone this repo and paste directiories "BOOT" and "OC" onto created directory
  3. Download [**GenSMBIOS**](https://github.com/corpnewt/GenSMBIOS) to generate unique SMBIOS information. Run it and select **Generate SMBIOS**, as model select **MacPro7,1**.
  4. Open config.plist with [**ProperTree**](https://github.com/corpnewt/ProperTree) and go to PlatformInfo > Generic. Set MLB (Board Serial), SystemSerialNumber (Serial) and SystemUUID (SmUUID) to generated values.
  5. Boot it!  

## Disclaimer

This documentation is published for the sole purpose of learning and tech enthusiasm and with no guarantees of any kind, I’m not responsible of any harm of any kind or loss of data that may occur.
