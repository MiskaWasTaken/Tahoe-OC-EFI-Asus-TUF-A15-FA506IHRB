# Tahoe OpenCore EFI – ASUS TUF A15 (Ryzen 5 4600H & GTX 1650)
💻 OpenCore EFI for running **macOS** on an **ASUS TUF A15** laptop with **Ryzen 5 4600H** and **GTX 1650**.  

> 🚧 **Work in Progress** – This guide will evolve as testing progresses.

## This config is very heavily dependant on your system, even if you have the same model as me, it might not work
There have been alot of mmiodevirt and SDDTime configs involved, proceed with caution as my efi might not work for you even if we have the same system config.

## Hardware Compatibility
This EFI is designed for the following configuration:  

### System Specifications
| **Component** | **Details** |
|-------------|------------|
| **Model** | ASUS TUF A15 |
| **CPU** | AMD Ryzen 5 4600H |
| **GPU** | NVIDIA GTX 1650 *(disabled, unsupported in macOS)* |
| **Integrated Graphics** | AMD Radeon (patched with NootedRed) |
| **RAM** | 16GB DDR4 |
| **Storage Slot 1** | Stock Samsung NVMe SSD (512GB) |
| **Wi-Fi & Bluetooth** | Unsupported |
| **Audio** | Unsupported/AppleHDA (Use OLCP-MOD for AppleALC) |
| **Ethernet** | RealtekRTL8111 |
| **SMBIOS** | MacBookPro16,2 |

## Booting macOS ⛔

To get past the **prohibitory symbol** during boot, you must:
1. SDDTime patch
2. MMIOdevirt
