[![](https://img.shields.io/badge/Gitter%20HL%20Community-Chat-informational?style=flat&logo=gitter&logoColor=white&color=ed1965)](https://gitter.im/Hackintosh-Life-IT/community)
[![](https://img.shields.io/badge/EFI-Release-informational?style=flat&logo=apple&logoColor=white&color=9debeb)](https://github.com/Lorys89/DELL_OPTIPLEX_9030_AIO/releases)
[![](https://img.shields.io/badge/Telegram-HackintoshLifeIT-informational?style=flat&logo=telegram&logoColor=white&color=5fb659)](https://t.me/HackintoshLife_it)
[![](https://img.shields.io/badge/Facebook-HackintoshLifeIT-informational?style=flat&logo=facebook&logoColor=white&color=3a4dc9)](https://www.facebook.com/hackintoshlife/)
[![](https://img.shields.io/badge/Instagram-HackintoshLifeIT-informational?style=flat&logo=instagram&logoColor=white&color=8a178a)](https://www.instagram.com/hackintoshlife.it_official/)
# Dell Optiplex 9030 AIO Hackintosh
EFI for Dell Optiplex 9030 All in One with OpenCore bootloader

![descrizione](./Screenshot/pc.jpg)

### Computer Spec:

| Component        | Brank                              |
| ---------------- | ---------------------------------- |
| CPU              | Intel i5 4590s (4C-4T 6MB HSW)     |
| iGPU             | Intel® HD Graphics 4600            |
| Lan              | Intel I217LM                       |
| Wifi + BT        | BCM94360HMB (AW-CB160H)            |
| Audio            | Realtek ALC280                     |
| Ram              | 16 GB DDR3 1600 Mhz                |
| SSD              | SAMSUNG 860 EVO 500 GB (WINDOWS)   |
| NVME             | NE - 256 GB (MACOS)                |
| SmBios           | MacMini 7,1                        |
| BootLoader       | OpenCore 0.7.1                     |
| macOS            | Monterey 12.0 (Beta 2)             |


![infomac](./Screenshot/infomac.png)

## Peripherals

![infohack](./Screenshot/periph.png)
![infodp2](./Screenshot/infopci.png)
![fan&temp](./Screenshot/fan&tempcontrol.png)
![ssd&ram](./Screenshot/ssd-ram.png)


### What works and What doesn't or WIP:

- [x] Intel HD Graphics 4600 iGPU HDMI/DP Output
- [x] ALC280 Internal Speakers
- [x] ALC280 Internal microphone
- [x] ALC280 HDMI/DP Audio Output
- [x] ALC280 front combojack HP/Mic
- [x] ALC280 rear jack speaker
- [x] Webcam FHD Internal
- [x] Slot SD card reader
- [x] All USB Ports 
- [x] All Sensors (CPU, IGPU, NVME, SATA, FAN, WIFI)
- [x] SpeedStep / Sleep / Wake
- [x] Native brightness side buttons
- [x] Intel I217LM LAN
- [x] Wi-Fi and Bluetooth BCM94360HMB (AW-CB160H) Module
- [x] HID Key PWRB & SLPB 
- [x] CONTROLLER SATA III
- [x] Internal Sata DVD-RW
- [x] CONTROLLER NVME
- [x] NVRAM
- [x] Windows 11 boot from OpenCore
- [x] Sidecar (thanks to the new kext)

### Special Config:

- Usb port mapping performed
- SSDT-Hack Essential patch

See [ioreg](./ioregmac.ioreg) for more clarification

### MacOS bootable USB creation:
- Read the Dortania guide for creating your USB from Windows or macOS
- [Guide Dortania](https://dortania.github.io/OpenCore-Install-Guide/installer-guide/) - USB creation


## Bios settings
### Enable :
* SATA Operation : AHCI
* Integrated NIC : Enable

### Disable : 
* Secure Boot
* Serial Port
* Legacy support
* Enable UEFI Network stack
* Computrace
* cfg lock and DVMT DO AT YOUR OWN RISK!!! It may brick your PC.


## Restart and at the opencore GUI, choose the modGRUBShell.efi (into Tools Folder)

![CFG-LOCK](./Screenshot/CFG-LOCK.png)

For set CFG LOCK Disabled

setup_var 0xDAF 0x00

![DMT-PRE](./Screenshot/DVMT-PRE.png)

For set DVMT PRE Allocated to 64 MB

setup_var 0x263 0x02


## Credits

- [Apple](https://apple.com) for macOS;
- [Acidanthera](https://github.com/acidanthera) for OpenCore and all the lovely hackintosh work.
- [Dortania](https://dortania.github.io/OpenCore-Install-Guide/config-laptop.plist/icelake.html) For great and detailed guides.
- [Hackintoshlifeit](https://github.com/Hackintoshlifeit) Support group for installation and post installation.
