# Dell Latitude 7390 EFI - macOS Ventura

[![Static Badge](https://img.shields.io/badge/macOS-Ventura-orange)](https://developer.apple.com/documentation/macos-release-notes/macos-13-release-notes)
[![Static Badge](https://img.shields.io/badge/OpenCore-0.8.8-blue)](https://github.com/acidanthera/OpenCorePkg/releases/tag/0.8.8)
[![Static Badge](https://img.shields.io/badge/License-MIT-purple)](/LICENSE)

Dell Latitude 7390 OpenCore EFI build for macOS Ventura v13.7.8. It also works wih macOS BigSur.

## Screenshot

<p>
<figure>
<img src="./screenshots/desktop.png" alt="macOS Ventura Desktop" />
<figcaption>Screenshot of the macOS Ventura Desktop</figcaption>
</figure>
</p>

## Specification

| Device            | Model                               | Status   |
| ----------------- | ----------------------------------- | -------- |
| CPU               | Intel Core i5-8350U                 | Works    |
| GPU               | Intel UHD Graphics 620              | Works    |
| Memory            | SK hynix 16GB DDR4 2400 MHz         | Works    |
| Drive             | Samsung 970 EVO Plus                | Works    |
| Audio             | Realtek ALC3246                     | Works    |
| WiFi & BT         | Intel Wireless-AC 8265NGW           | Partial  |
| Ethernet          | Intel Ethernet I219-LM              | Works    |
| SD Card Reader    | Realtek RTS525A                     | Works    |
| Smart Card Reader | Broadcom USH 5880                   | Untested |
| Mic               | Builtin                             | Works    |
| Webcam            | Builtin                             | Works    |

## BIOS

The BIOS had been upgraded to v1.44.0 and following settings has been changed in order to make the installation process smoother.

<details>
<summary><strong>BIOS Options</strong></summary><br/>
<ul>
<li>Integrated NIC - Enabled</li>
<li>SATA Operation - AHCI</li>
<li>Keyboard Illumination - Disabled</li>
<li>Touchscreen - Unchecked</li>
<li>Absolute - Disabled</li>
<li>Secure Boot Enable - Unchecked</li>
<li>Secure Boot Mode - Audit Mode</li>
<li>Intel SGX Enable - Disabled</li>
<li>Wakes on LAN/WLAN - LAN Only</li>
<li>Block Sleep - Unchecked</li>
<li>Fastboot - Minimal</li>
<li>Intel AMT Capability - Enabled</li>
<li>UEFI Boot Path Security - Always, Except Internal HDD</li>
<li>Virtualization - Enable Intel Virtualization Technology</li>
<li>VT for Direct I/O - Enable VT for Direct I/O</li>
<li>Trusted Execution - Checked</li>
</ul>
</details>

## Notes

<details>
<summary><strong>Audio Issue</strong></summary><br/>
Correct audio <code>layout-id</code> is crucially important for your audio device to work properly, so spent sometime to figure it out. Check the AppleALC <a href="https://github.com/acidanthera/AppleALC/wiki/Supported-codecs">supported codec</a> page which covers wide range of audio devices.
</details>

<details>
<summary><strong>Generate SMBIOS</strong></summary><br/>
Please do not use my SMBIOS included within this EFI. Feel free to generate your own SMBIOS with <a href="https://github.com/ic005k/OCAuxiliaryTools">OCAT</a> or any other tool that you are familiar with.
</details>

## Credits

- [Acidanthera](https://github.com/acidanthera) - OpenCorePkg
- [OpenIntelWireless](https://github.com/OpenIntelWireless) - Intel Wireless Kexts
- [ic005k](https://github.com/ic005k) - OC Auxiliary Tools
- [corpnewt](https://github.com/corpnewt/) - ProperTree
- [badges](https://github.com/badges) - Shields.io