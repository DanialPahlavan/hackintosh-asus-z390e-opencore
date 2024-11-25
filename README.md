# hackintosh-ASUS-ROG-STRIX-Z390-E

> **Warning:** This project is for educational purposes only. Any violations and all risks are your own responsibility.

## System Information

```
HomeLab iMac iMac19.1 (Clone)
----------------------------------------------
Motherboard Model: ASUS ROG STRIX Z390-E GAMING
Operating System  : macOS 15.1.1 (Sequoia)
Processor         : Intel Core i9-9900K 3.60GHz x 16
Memory            : 32 GB (G.Skill DDR4)
Storage           : SamSung SSD 970 EVO Plus 500GB
Network Card      : Intel Wireless-AC 9560
Graphics          : Intel UHD Graphics 630 / VRAM (Dynamic, Max): 2048 MB
Primary Display   : LG 29 UltraWide
Sound Card        : Intel High Definition Audio Controller
```

## OpenCore Bootloader

This EFI is configured according to the [OpenCore Install Guide](https://dortania.github.io/OpenCore-Install-Guide/).

> **Note:** Backup your system before making any changes.
>
> **Note:** Ensure to copy the entire folder.

### Versions

- **BIOS:** 2101
- **OpenCore:** 1.0.2
- **macOS:** 15.1.1 (Sequoia)

### Prerequisites

- **Disable:**
  - Fast Boot
  - Launch CSM
  - Secure Boot
    - Key Management
      - Clear Secure Boot Keys
  - System Agent (SA) Configuration
    - VT-d
  - CFG Lock
  - Onboard Devices Configuration
    - Serial Port Configuration
      - Serial Port: Off

- **Enable:**
  - System Agent (SA) Configuration
    - Above 4G Decoding
    - Graphics Configuration
      - Primary Display: CPU Graphics
      - DVMT Pre-Allocated: 64MB
  - CPU Configuration
    - Hyper-Threading
  - USB Configuration
    - XHCI Hand-off
  - Secure Boot
    - OS Type: OtherOS

### Credits

- picopock

