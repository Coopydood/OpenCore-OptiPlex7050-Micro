
<img align="left" height="150" src="https://github.com/user-attachments/assets/b0fce891-4de1-4397-b330-923c316abc65">

<img align="left" src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/8f69f9b9-cf23-4e8b-adf3-95862a23e2ba" height=210 width=1 />

<a href="https://coopydood.github.io/ultimate-macOS-KVM"></a><h3>OpenCore OptiPlex 7050 Micro (Kaby Lake)</h3>

OpenCore Hackintosh configuration example for the **Dell OptiPlex 7050 Micro Form Factor** with an Intel® Core™ i5-7500. 
<br>

[![GitHub](https://img.shields.io/github/license/Coopydood/OpenCore-OptiPlex7050-Micro?label=Licence&logo=unlicense&logoColor=white&style=for-the-badge)](https://github.com/Coopydood/OpenCore-OptiPlex7050-Micro/blob/main/LICENSE) [![GitHub repo size](https://img.shields.io/github/repo-size/Coopydood/OpenCore-OptiPlex7050-Micro?color=07b55b&label=Size&logo=envoy-proxy&logoColor=white&style=for-the-badge)](https://github.com/Coopydood/OpenCore-OptiPlex7050-Micro) [![Discord](https://img.shields.io/discord/574943603466436628?color=7d86ff&label=Discord&logo=discord&logoColor=white&style=for-the-badge)](https://discord.gg/WzWkSsT)

<br><br>

***

## OpenCore

<img align="left" width="100" height="100" src="https://dortania.github.io/docs/latest/Logos/Logo.png">
<img align="left" src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/8f69f9b9-cf23-4e8b-adf3-95862a23e2ba" height=100 width=2 />
<h3>OpenCore<br><sub>1.0.0</sub></h3>

This is the version of OpenCore used, including bundled files. The included ``config.plist`` targets this version.
<br>


## macOS

<img align="left" width="90" height="90" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/aa49b5ba-6cca-4dab-bcfc-6bf21909e738">
<!-- CHANGE THE IMAGE URL TO THE MAIN OS YOUR CONFIG TARGETS. IMAGE URL LIST BELOW! -->

<img align="left" src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/8f69f9b9-cf23-4e8b-adf3-95862a23e2ba" height=520 width=2 /> 
<!-- CHANGE THE HEIGHT WHEN ADDING OR REMOVING SUPPORTED OSES TO THE LIST (Default: 520) -->

<h3>macOS Sonoma<br><sub>14.5</sub></h3>

This is the version of macOS that this OpenCore configuration currently targets. Other versions of macOS that are compatible with it are listed below.<br>

#### Supported

<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/4829ebb4-ce7f-4ecf-8309-d691c9361f6b"> 
<h5>macOS Ventura</h5>
<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/7d341cce-4370-4430-b3d5-bf1868afe4a3"> 
<h5>macOS Monterey</h5>
<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/79a7a051-0f5a-419e-8544-b51b1572d3b9"> 
<h5>macOS Big Sur</h5>
<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/cd8029e8-c256-4295-9908-37809d64dcfe"> 
<h5>macOS Catalina</h5>
<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/184bb2ef-c447-4cbd-b07c-8b4b096e3944"> 
<h5>macOS Mojave</h5>
<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/bd4a791d-1ac2-4a9a-8ee0-22e4d5f88cd3"> 
<h5>macOS High Sierra</h5>
<img align="left" width="35" height="35" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/788860d8-207a-4d15-928a-ed78f08962cf"> 
<h5>macOS Sierra</h5>

<br>

***


## What works?

### macOS

- [x] macOS Sonoma

### Hardware

- [x] iGPU (Intel HD 630)
- [x] SATA drive
- [x] USB 3.1 (XHCI)
- [x] Ethernet
- [x] Wi-Fi
- [x] Bluetooth
- [x] Sound
  
### Software

- [x] AirDrop
- [x] iMessage
- [x] FaceTime
- [x] Unlock with Apple Watch
- [x] QE/CI graphics acceleration
- [x] Metal support
- [x] Temperature sensors
- [ ] Sleep / Wake
- [ ] Hyperthreading
- [x] Virtualisation
- [x] Memory bank configuration
  
<br>

***

## Problems

<ul>
<li><b>TBD</b></li>
TBD

</ul>


***

## System

The specs of the main system that the OpenCore configuration targets.

| **Motherboard** |                  Dell                 |
|-----------------|:-------------------------------------------------------------:|
| **CPU**         |                      Intel® Core™ i5-7500                     |
| **Chipset**     |                             OptiPlex 7050                            |
| **Generation**  |                           Kaby Lake                          |
| **Memory**      |                       8 GB DDR4                       |
| **Storage**     |                     256 GB SATA SSD                    |
| **GPU**         | Intel HD 630 |
| **NIC**         |                  Intel I219-LM                  |

***

## ACPI

SSDTs used:
- SSDT-1
- SSDT-2
- SSDT-3
  
***

## DeviceProperties

The following tables display the added PCI devices and their child keys.


### PciRoot(0x0)/Pci(0x2,0x0)

EXAMPLE

| **Key**                  | **Type** |   **Value**  |
|--------------------------|:--------:|:------------:|
| AAPL,ig-platform-id      |   Data   | ``0000923E`` |
| device-id                |   Data   | ``923E7000`` |
| framebuffer-fbmem        |   Data   | ``00009000`` |
| framebuffer-patch-enable |   Data   | ``01000000`` |
| framebuffer-stolenmem    |   Data   | ``00003001`` |
| framebuffer-unifiedmem   |   Data   | ``00000080`` |
| hda-gfx                  |  String  |   onboard-1  |

<br>

### PciRoot(0x0)/Pci(0x1b,0x0)

Apple ALC

| **Key**                  | **Type** |   **Value**  |
|--------------------------|:--------:|:------------:|
| AAPL,ig-platform-id      |   Data   | ``0300220D`` |
| layout-id                |   Data   | ``01000000`` |


***

## Kernel

The following shows the kernel configuration.

### Kexts

Kexts used:
- Lilu
- WhateverGreen
- ...


### Patches

None

***

## Security

**SecureBootModel 》** SECURE_BOOT_MODEL

**Vault 》** Optional


***

## NVRAM

Contents stored in NVRAM.

<br>

### 4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14

| **Key**                | **Type** |   **Value**  |
|------------------------|:--------:|:------------:|
| DefaultBackgroundColor |   Data   | ``00000000`` |

<br>

### 4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102

| **Key**       | **Type** | **Value** |
|---------------|:--------:|:---------:|
| rtc-blacklist |   Data   |           |

<br>

### 7C436110-AB2A-4BBB-A880-FE41995C9F82

| **Key**                   | **Type** |                                    **Value**                                   |
|---------------------------|:--------:|:------------------------------------------------------------------------------:|
| boot-args                 |  String  | TBD |

***

## SMBIOS

### TBD

TBD

***



## UEFI

Drivers in use:

- HFSPlus
- OpenRuntime
- ...
  
***

## Gallery

TBD

***

## Disclaimer

TBD

