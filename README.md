# Fully Functional Asus X570 TUF Gaming Plus/BR Hackintosh

![Ryzentosh_CCSilvs](https://github.com/CCSilvs/EFI-ASUS-TUF-GAMING-X570-PLUS-BR-/assets/91890693/57eed575-af01-4a04-9dab-e0d61e65f96a)

**MacOS version:** Ventura 13.6
<br>
**OpenCore version:** 0.9.5

## **Specs**
| **Component** | **Model** |
| ------------- | --------- |
| CPU | AMD Ryzen 7 5700X |
| Motherboard | ASUS TUF Gaming X570-PLUS/BR |
| GPU | PowerColor Radeon RX 6800 XT 16GB GDDR6 Red Dragon |
| RAM | 32GB Geil EVO X 3200MHz C16 (4x8GB) |
| WAN | Fenvi T919 1750Mbps (BCM94360CD) |
| LAN CHIPSET | Realtek® L8200A Gigabit LAN |
| AUDIO CHIPSET | Realtek® ALC S1200A |
| STORAGE MacOS | 1TB Adata XPG Gammix S70 Blade PCIe 4.0 7400/6800MB/s (r/w) |
| STORAGE Windows | 1TB Adata XPG SX8200 PCIe 3.0 3500/300MB/s (r/w) |
| CPU Cooler | Scythe Fuma 3 + third Fan |
| PSU | XPG Core Reactor 850W, 80 Plus Gold Modular |
| CASE | Corsair ICUE 5000X White |
| COOLING | 3x3 fan kits by Corsair, Coolermaster & Thermalright |
| SCREEN 1 | Horizontal: LG 29UM69G - 29" Ultrawide (2560x1080px) | 
| SCREEN 2 | Vertical: Ozone OZDSP28IPS - 28" Standard (3840x2160px) |

## **What works**
- All MacOS since Big Sur to Ventura (Sonoma in the next Opencore update)
- Audio: front panel, rear panel including Optic Digital Out
- All USB ports
- Wifi, Bluetooth, Airdrop, Airplay (even with Samsung TV screens), Sidecar
- Everything from iCloud and Apple phones, pads & gadgets
- Temperature monitoring for everything includes GPU
- Sleep/wake up

## **What doesn't work**
- Microphone and line in on rear panel (know AMD issue)

## ACPI used:
- SSDT-EC-USBX-DESKTOP.aml (prebuild)
  
## Opencore Drivers:
- AudioDxe.efi
- HfsPlus.efi
- OpenCanopy.efi
- OpenRuntime.efi
- ResetNvramEntry.efi
- ToggleSipEntry.efi

## Kexts used:
- AMDRyzenCPUPowerManagement.kext
- AppleALC.kext
- AppleMCEReporterDisabler.kext
- FeatureUnlock.kext
- HibernationFixup.kext
- Lilu.kext
- NVMeFix.kext
- RadeonSensor.kext
- RealtekRTL8111.kext
- RestrictEvents.kext
- SMCAMDProcessor.kext
- SMCRadeonGPU.kext
- VirtualSMC.kext
- WhateverGreen.kext

## BIOS Settings

**Disable**
- Fast Boot
- Secure Boot
- Serial/COM Port
- Compatibility Support Module (CSM)

**Enable**
- Above 4G decoding
- Resizable BAR can be set "Auto", this config.plist already has a setting to mantaing this option enabled to guarantee the best graphical performance in Windows
- EHCI/XHCI Hand-off
- OS type: Windows 8.1/10 UEFI Mode
- SATA Mode: AHCI

## Geekbench results
CPU <br>
<img width="850" alt="Screenshot 2023-10-24 at 21 58 41" src="https://github.com/CCSilvs/EFI-ASUS-TUF-GAMING-X570-PLUS-BR-/assets/91890693/6da6f4d3-0929-4f29-9cb1-a49c3b3895b6">

GPU <br>
<img width="851" alt="Screenshot 2023-10-24 at 21 59 17" src="https://github.com/CCSilvs/EFI-ASUS-TUF-GAMING-X570-PLUS-BR-/assets/91890693/e25f791d-7985-4a24-acaa-9850156ed9b8">

## Credits
- <p>Special thnx to <a href="https://github.com/luchina-gabriel/"> Gabriel Luchina</a></p>
- <p>His knowledge and repository <a href="https://github.com/luchina-gabriel/BASE-EFI-AMD-RYZEN-THREADRIPPER/"> BASE-EFI-AMD-RYZEN-THREADRIPPER</a></p>

- [Opencore Team](https://dortania.github.io/getting-started/)
