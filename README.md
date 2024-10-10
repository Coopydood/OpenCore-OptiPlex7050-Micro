<img align="left" height="150" src="https://github.com/user-attachments/assets/b0fce891-4de1-4397-b330-923c316abc65">

<img align="left" src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/8f69f9b9-cf23-4e8b-adf3-95862a23e2ba" height=210 width=1 />

<a href="https://coopydood.github.io/ultimate-macOS-KVM"></a><h3>OpenCore OptiPlex 7050 Micro (Kaby Lake)<br><sub>v1.0.1</sub></h3>

OpenCore Hackintosh configuration example for the **Dell OptiPlex 7050 Micro Form Factor** with an Intel® Core™ i5-7500T. 
<br>

[![GitHub](https://img.shields.io/github/license/Coopydood/OpenCore-OptiPlex-7060?label=Licence&logo=unlicense&logoColor=white&style=for-the-badge)](https://github.com/Coopydood/OpenCore-OptiPlex-7060/blob/main/LICENSE) [![GitHub repo size](https://img.shields.io/github/repo-size/Coopydood/OpenCore-OptiPlex-7060?color=07b55b&label=Size&logo=envoy-proxy&logoColor=white&style=for-the-badge)](https://github.com/Coopydood/OpenCore-OptiPlex-7060) [![Discord](https://img.shields.io/discord/574943603466436628?color=7d86ff&label=Discord&logo=discord&logoColor=white&style=for-the-badge)](https://discord.gg/WzWkSsT)

<br>

***

<img src="https://github.com/user-attachments/assets/7c066696-4b71-41aa-8f79-f51d538f9666" alt="cute lil OptiPlex 7050 Micro" width="1400"/><br>
<p align="center"><i>The cute lil 7050 Micro running macOS!</i></p>


***

## OpenCore

<img align="left" width="100" height="100" src="https://dortania.github.io/docs/latest/Logos/Logo.png">
<img align="left" src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/8f69f9b9-cf23-4e8b-adf3-95862a23e2ba" height=100 width=2 />
<h3>OpenCore<br><sub>1.0.2</sub></h3>

This is the version of OpenCore used, including bundled files. The included ``config.plist`` targets this version.
<br>


## macOS

<img align="left" width="90" height="90" src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/aa49b5ba-6cca-4dab-bcfc-6bf21909e738">
<!-- CHANGE THE IMAGE URL TO THE MAIN OS YOUR CONFIG TARGETS. IMAGE URL LIST BELOW! -->

<img align="left" src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/8f69f9b9-cf23-4e8b-adf3-95862a23e2ba" height=520 width=2 /> 
<!-- CHANGE THE HEIGHT WHEN ADDING OR REMOVING SUPPORTED OSES TO THE LIST (Default: 520) -->

<h3>macOS Sonoma<br></h3>

This is the version of macOS that this OpenCore configuration currently targets. Other versions of macOS that are compatible with it are listed below.<br>

#### Supported

<img align="left" width="35" height="35" src="https://github.com/user-attachments/assets/7b9b72ee-5a89-49b4-ae17-7a188ed533ab"> 
<h5>macOS Sequoia</h5>
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

<br>

<br><br>


***


## What works?

### macOS

- [x] macOS Sonoma

### Hardware

- [x] iGPU (Intel HD Graphics 630)
- [x] NVMe drive
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
- [x] Boot chime
  
<br>

***

## Problems

<ul>
<li><b>Sleep / Wake</b></li>
Unfortunately, sleep is broken on this system at the moment. The system itself can go into and out of the sleep state, but the monitor never wakes up. My <a href="https://github.com/Coopydood/OpenCore-OptiPlex7060-SFF">other OptiPlex hacc</a> does this too. I'll investigate this!
  
<br><br>

<li><b><s>External Audio and HDMI Output</s> ‏‏‎ ‏‏‎ ‎‎‏‏‎ ‎ 🎉 FIXED!</b></li>
<s>Unfortunately, external audio - both DisplayPort and HDMI - doesn't work. HDMI output is also broken, with the system failing to boot with only HDMI plugged in. Strangely, once booted, the system does half-work with HDMI, but is locked at low resolution.</s>

> [!TIP]
> This was fixed by using a combo of DeviceProperties entries from <a href="https://github.com/AurelienAudero/Intel-i5-7400-Hackintosh-EFI">this excellent repo</a>!

<br><br>

<li><b><s>VGA Output</s> ‏‏‎ ‏‏‎ ‎‎‏‏‎ ‎ 🎉 FIXED!</b></li>
<s>The "option port" of my 7050 happens to be a jurassic-era VGA connector. As probably expected, macOS doesnt work with the VGA port.</s>

> [!TIP]
> This was fixed using custom connector patches in DeviceProperties!

</ul>


***

## System

The specs of the main system that the OpenCore configuration targets.

| **Motherboard** |                  Dell                 |
|-----------------|:-------------------------------------------------------------:|
| **CPU**         |                      Intel® Core™ i5-7500T                     |
| **Chipset**     |                             OptiPlex 7050 MFF                            |
| **Generation**  |                           Kaby Lake                          |
| **Memory**      |                       16 GB 2400MHz DDR4                       |
| **Storage**     |                     256 GB NVMe SSD<br>256 GB SATA SSD                    |
| **GPU**         | Intel HD Graphics 630 |
| **NIC**         |                  Intel I219-LM                  |

<br>

### Geekbench Scores

| **Intel Core i5-7500T** | **macOS** |
|-------------------------|-----------|
| Single Core             | 1,153     |
| Muti Core               | 3,371     |

| **GPU**                  | **macOS**<br>Metal |
|--------------------------|--------------------|
| Intel<br>HD 630 Graphics | 5,984              |

<br>

***

## ACPI

SSDTs used:
- SSDT-EC-USBX-DESKTOP
- SSDT-HPET *
- SSDT-PLUG

> [!IMPORTANT]
> ``SSDT-HPET`` was compiled by me specifically for this machine model. Along with several ACPI patches, this is used to fix **onboard audio, including internal speakers.** Without it, macOS will show as having no built-in audio devices.  
  
***

## DeviceProperties

The following tables display the added PCI devices and their child keys.

### PciRoot(0x0)/Pci(0x1F,0x3)

Internal Speakers

| **Key**                  | **Type** |   **Value**  |
|--------------------------|:--------:|:------------:|
| AAPL,slot-name           |   String | ``Internal@0,31,3`` |
| device_type              |   String | ``Audio device`` |
| model                  |   String   | ``200 Series PCH HD Audio`` |
| layout-id                |   Data   | ``11000000`` |

<details><summary><h4>📄  Show as property list data</h4><br><sup>Expand this if you want to copy and paste the entries above as <code>.plist</code> data!</summary>

You can paste this data straight into plist editors like ProperTree.

```xml
<key>PciRoot(0x0)/Pci(0x1F,0x3)</key>
<dict>
  <key>AAPL,slot-name</key>
  <string>Internal@0,31,3</string>
  <key>device_type</key>
  <string>Audio device</string>
  <key>layout-id</key>
  <data>EQAAAA==</data>
  <key>model</key>
  <string>200 Series PCH HD Audio</string>
</dict>
```
</details><br>

<br>

### PciRoot(0x0)/Pci(0x2,0x0)

Intel HD Graphics 630

| **Key**                  	| **Type** 	| **Value**                 	|
|--------------------------	|:----------:|:---------------------------:|
| AAPL,ig-platform-id      	|   Data   	|        ``00001259``       	|
| device-id                	|   Data   	|        ``1B590006``       	|
| disable-agdc             	|   Data   	|        ``01000000``       	|
| enable-hdmi-dividers-fix 	|   Data   	|        ``01000000``       	|
| enable-hdmi20            	|   Data   	|        ``01000000``       	|
| framebuffer-con0-enable  	|   Data   	|        ``01000000``       	|
| framebuffer-con0-alldata    	|   Data   	|        ``01050900 00080000 87010000``       	|
| framebuffer-con1-enable  	|   Data   	|        ``01000000``       	|
| framebuffer-con1-alldata    	|   Data   	|        ``02040A00 00040000 87010000``       	|
| framebuffer-con2-enable  	|   Data   	|        ``01000000``       	|
| framebuffer-con2-alldata    	|   Data   	|        ``03060A00 00040000 87010000``       	|
| framebuffer-patch-enable 	|   Data   	|        ``01000000``       	|
| framebuffer-stolenmem    	|   Data   	|        ``00003001``       	|
| rps-control              	|   Data   	|        ``01000000``       	|
| model                    	|  String  	| ``Intel HD Graphics 630`` 	|

<details><summary><h4>📄  Show as property list data</h4><br><sup>Expand this if you want to copy and paste the entries above as <code>.plist</code> data!</summary>

You can paste this data straight into plist editors like ProperTree.

```xml
<key>PciRoot(0x0)/Pci(0x2,0x0)</key>
<dict>
  <key>AAPL,ig-platform-id</key>
  <data>AAASWQ==</data>
  <key>device-id</key>
  <data>G1kABg==</data>
  <key>device_type</key>
  <string>VGA compatible controller</string>
  <key>disable-agdc</key>
  <data>AQAAAA==</data>
  <key>enable-hdmi-dividers-fix</key>
  <data>AQAAAA==</data>
  <key>enable-hdmi20</key>
  <data>AQAAAA==</data>
  <key>framebuffer-con0-alldata</key>
  <data>AQUJAAAIAACHAQAA</data>
  <key>framebuffer-con0-enable</key>
  <data>AQAAAA==</data>
  <key>framebuffer-con1-alldata</key>
  <data>AgQKAAAEAACHAQAA</data>
  <key>framebuffer-con1-enable</key>
  <data>AQAAAA==</data>
  <key>framebuffer-con2-alldata</key>
  <data>AwYKAAAEAACHAQAA</data>
  <key>framebuffer-con2-enable</key>
  <data>AQAAAA==</data>
  <key>framebuffer-patch-enable</key>
  <data>AQAAAA==</data>
  <key>framebuffer-stolenmem</key>
  <data>AAAwAQ==</data>
  <key>model</key>
  <string>Intel HD Graphics 630</string>
  <key>rps-control</key>
  <data>AQAAAA==</data>
</dict>
```
</details><br>

> [!NOTE]
> The framebuffer connector patching was done using [this section of the WhateverGreen Intel guide](https://github.com/acidanthera/WhateverGreen/blob/master/Manual/FAQ.IntelHD.en.md#intel-uhd-graphics-610-650-kaby-lake-and-amber-lake-y-processors) as a reference.

> [!TIP]
> The ``device-id`` has been set to ``1B590006`` as this fixes up some string-related cosmetics around macOS - such as changing the Metal device name from ``Intel KBL Unknown`` to ``Intel HD Graphics 630``.
> 
> The previous ``device-id`` (``12590000``) matches more closely but has the aforementioned cosmetic issues. Both IDs work absolutely fine.

<br>


***

## Kernel

The following shows the kernel configuration.

### Kexts

Kexts used:
- Lilu
- WhateverGreen
- AppleALC
- IntelMausi
- RestrictEvents
- RTCMemoryFixup
- SMCProcessor
- SMCSuperIO
- SMCDellSensors
- VirtualSMC
- HibernationFixup
- FeatureUnlock
- IntelBluetoothFirmware
- IntelBTPatcher
- BlueToolFixup
- OptiPlex7050_MFF_USBMap *
- ~~USBMapDummy~~

> [!IMPORTANT]
> The ``OptiPlex7050_MFF_USBMap.kext`` is the USB map created manually by me on my own system. It may or may not work for other 7050 Micro machines. If it doesn't work, please disable it.

> [!TIP]
> In case you need it for your own mapping, ``USBMapDummy.kext`` has been left included but disabled, so you can enable it if you need it.


### Patches

None

***

## Security

**SecureBootModel 》** ``j174``

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
| ForceDisplayRotationInEFI |  Number  |                                        0                                       |
| SystemAudioVolume         |   Data   |                                     ``46``                                     |
| boot-args                 |  String  | keepsyms=1 debug=0x100 -cdfon -igfxmpc -igfxcdc igfxrpsc=1 itlwm_cc=GB revpatch=sbvmm |
| csr-active-config         |   Data   |                                  ``00000000``                                  |
| prev-lang-diags:kbd       |   Data   |                                 ``656E2D47 42``                                |
| prev-lang:kbd             |   Data   |                               ``656E2D47 423A32``                              |                                      |
| StartupMute               |   Data   |                                     ``00``                                     |

<details><summary><h4>📄  Show as property list data</h4><br><sup>Expand this if you want to copy and paste the entries above as <code>.plist</code> data!</summary>

You can paste this data straight into plist editors like ProperTree.

```xml
<key>4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14</key>
<dict>
  <key>DefaultBackgroundColor</key>
  <data>AAAAAA==</data>
</dict>
<key>4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102</key>
<dict>
  <key>rtc-blacklist</key>
  <data></data>
</dict>
<key>7C436110-AB2A-4BBB-A880-FE41995C9F82</key>
<dict>
  <key>ForceDisplayRotationInEFI</key>
  <integer>0</integer>
  <key>SystemAudioVolume</key>
  <data>Rg==</data>
  <key>boot-args</key>
  <string>keepsyms=1 debug=0x100 -cdfon -igfxmpc -igfxcdc igfxrpsc=1 itlwm_cc=GB revpatch=sbvmm</string>
  <key>prev-lang-diags:kbd</key>
  <data>ZW4tR0I=</data>
  <key>prev-lang:kbd</key>
  <data>ZW4tR0I6Mg==</data>
  <key>csr-active-config</key>
  <data>AAAAAA==</data>
  <key>run-efi-updater</key>
  <string>No</string>
  <key>fmm-computer-name</key>
  <string>iPlex mini</string>
</dict>
```
</details><br>

***

## SMBIOS

### Macmini8,1

As it's a cute lil boi, it makes sense to have it emulate a Mac mini, even though its closest SMBIOS would be the ``iMac18,2`` - which isn't even supported anymore.

***



## UEFI

Drivers in use:

- HFSPlus
- OpenRuntime
- OpenCanopy
- AudioDxe *

>[!NOTE]
``AudioDxe`` is loaded so that OpenCore can make a boot chime on startup!
  
***

## Post-Install Tweaks

This is just a collection of my post-install tweaks I apply after installing macOS. They're not really related to OpenCore or the overall functionality of the configuration.

<details><summary><h4>Dark Menu Bar and Dock</h4></summary>

Okay, so I'm a bit of a macOS boomer. Having used macOS since long before Mojave's *dark mode*, I'm accustomed to the regular light appearance of the windows - but I always enabled the "Dark menu bar and dock" option as I loved the look. While I still like dark mode (and use it on iOS), the hybrid light/dark mode on macOS is still my favourite!

The following commands restore that functionality:

**Window Server**
```sh
defaults write -g NSRequiresAquaSystemAppearance -bool Yes
```

**Notification Centre**
```sh
defaults write com.apple.notificationcenterui NSRequiresAquaSystemAppearance -bool No
```

**Control Centre**
```sh
defaults write com.apple.controlcenterui NSRequiresAquaSystemAppearance -bool No
```

**About This Mac + System Profiler**
```sh
defaults write com.apple.SystemProfiler.AboutExtension NSRequiresAquaSystemAppearance -bool No
defaults write com.apple.SystemProfiler.AboutExtension NSRequiresAquaSystemAppearance -bool No
```

</details>

<details><summary><h4>Show Hidden Files</h4></summary>

Does what it says on the tin. Shows all files, including hidden ones, in the Finder.

```sh
defaults write com.apple.Finder AppleShowAllFiles YES
killall Finder
```
</details>


<details><summary><h4>AirDrop over Ethernet</h4></summary>

Makes AirDrop scan Ethernet too!

```sh
defaults write com.apple.NetworkBrowser BrowseAllInterfaces 1
killall Finder
```
</details>

<details><summary><h4>Frosted Glass Terminal Theme</h4></summary>

Some macOS eye candy.

```sh
curl -OL https://raw.githubusercontent.com/Coopydood/OpenCore-Z490E-CometLake/main/EXTRAS/HyperTerm.terminal
```

Import through Terminal's preferences.
</details>


***

## Gallery
<img src="https://github.com/user-attachments/assets/4cb5b688-1888-4ef7-b5e2-c071d051d5df" alt="cute lil OptiPlex 7050 Micro" width="1050"/><br><br>
<img src="https://github.com/user-attachments/assets/6b8eccff-201e-426a-8550-50ed8c49445e" width="30%"></img> <img src="https://github.com/user-attachments/assets/8a2104c2-9ce6-4e85-a11f-c3ed9727b0bb" width="60%"></img> <img src="https://github.com/user-attachments/assets/7b29f8a0-4f29-46f6-9707-48746f4947d4" width="45%"></img> <img src="https://github.com/user-attachments/assets/ff6e717a-3f27-4f0d-9224-6b3c7da3f777" width="45%"></img> <img src="https://github.com/user-attachments/assets/358c3746-3b55-4f46-b0dd-053d55f4c0c0" width="45%"></img> <img src="https://github.com/user-attachments/assets/0718cacf-50c7-4dfa-aa36-be3a36b01089" width="45%"></img> <img src="https://github.com/user-attachments/assets/a09a2306-59d2-4b41-906c-401386fa8788" width="45%"></img> <img src="https://github.com/user-attachments/assets/c7170196-c95b-436f-9bc7-365ba2a0e69b" width="45%"></img>

***

## Disclaimer

This repo is simply a dump of my current and up-to-date OpenCore stuff that I use on my machine. 

Feel free to use it as an example and modify it however you'd like, but please don't expect it to "just work" - because it *probably* won't.

***

## Contribute!

If you've found a way to make the configuration better, or have solved issues outlined in the **Problems** section, please share your changes on GitHub for us all to use! Thank you!

***

<p align="center">
  <img src="https://github.com/Coopydood/ultimate-macOS-KVM/assets/39441479/39d78d4b-8ce8-44f4-bba7-fefdbf2f80db" width="10%"> </img>
</p>
