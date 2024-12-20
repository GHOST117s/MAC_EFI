## Translation Request: A Comprehensive macOS Hackintosh Software and Driver List

**Prompt Analysis:**
The provided Chinese text is essentially a curated list of software and drivers commonly used for creating a Hackintosh, a non-Apple computer running macOS. The list is categorized into three sections:

* **Software:** Tools for configuring and managing the Hackintosh system.
* **Drivers:** Kernel extensions (kexts) that provide compatibility for various hardware components.
* **To be continued:** Indicates that the list is incomplete and will be expanded upon.

**Translation Notes:**
* **Technical Terms:** Many terms in this list are specific to macOS and Hackintoshing. I've provided common English equivalents where possible, but some terms might require further context for a complete understanding.
* **Links:** The links provided in the Chinese list are to specific repositories or download pages for each software or driver. These links will remain in the English translation for easy reference.

### English Translation

## 1. Software

| Software Name             | Link                                     | Primary Purpose                                     |
| ---------------- | ---------------------------------------- | ---------------------------------------- |
| Clover  | [Link](https://sourceforge.net/projects/cloverefiboot)  | EFI boot loader, foundation for ACPI code loading and related drivers  |
| Clover Configurator  | [Link](https://mackie100projects.altervista.org/download-clover-configurator)  | Clover configuration tool, remember to update frequently  |
| DarwinDumper  | [Link](https://bitbucket.org/blackosx/darwindumper/downloads)  | Similar to AIDA64, a very useful tool, but not widely used, which is a pity  |
| Hackintool  | [Link](https://www.insanelymac.com/forum/topic/335018-hackintool-v224)  | Patches Framebuffer, enables custom USB port configuration, and selects AppleALC layout-id nodes  |
| IORegistryExplorer  | [Link](https://www.tonymacx86.com/attachments/ioregistryexplorer-slrid_v10-6-3-zip.24086)  | Views system I/O information and the relationships between drivers and devices  |
| MaciASL  | [Link](https://github.com/acidanthera/MaciASL/releases)  | AML compiler and IDE, used to modify DSDT and create hot patches  |
| OSX-Debug  | [Link](https://github.com/black-dragon74/OSX-Debug)  | Script for collecting raw ACPI tables, drivers, crash logs, and other relevant information, used to provide feedback to developers  |
| ProperTree | [Link](https://github.com/corpnewt/ProperTree)  | OpenCore's officially recommended configuration tool | 

## 2. Drivers

### Lilu and Its Plugins

| Driver Name             | Link                                     | Primary Purpose                                     |
| ---------------- | ---------------------------------------- | ---------------------------------------- |
| Lilu  | [Link](https://github.com/acidanthera/Lilu)  | Driver injection framework, dependency for AppleALC, WhateverGreen, VirtualSMC, and other drivers  |
| AirportBrcmFixup  | [Link](https://github.com/acidanthera/AirportBrcmFixup)  | Broadcom wireless network card driver  |
| AppleALC  | [Link](https://github.com/acidanthera/AppleALC)  | Sound card injection framework  |
| ATH9KFixup  | [Link](https://github.com/chunnann/ATH9KFixup)  | Atheros network card driver  |
| BT4LEContiunityFixup  | [Link](https://github.com/acidanthera/BT4LEContiunityFixup)  | Enables Handoff, AirDrop, and other features  |
| CPUFriend  | [Link](https://github.com/acidanthera/CPUFriend)  | Injects dynamic power data for the CPU  |
| DiskArbitrationFixup | [Link](https://github.com/Goldfish64/DiskArbitrationFixup)  | Disables the "This computer cannot read the disk you inserted" prompt  |
| HibernationFixup  | [Link](https://github.com/acidanthera/HibernationFixup)  | Fixes hibernation issues  |
| NightShiftUnlocker | [Link](https://github.com/0xFireWolf/NightShiftUnlocker)  | Enables Night Shift feature  |
| NoTouchID  | [Link](https://github.com/al3xtjames/NoTouchID)  | Disables Touch ID support  |
| SystemProfilerMemoryFixup | [Link](https://github.com/Goldfish64/SystemProfilerMemoryFixup)  | Displays the memory label about this machine  |
| VirtualSMC  | [Link](https://github.com/acidanthera/VirtualSMC)  | SMC emulation driver, choose between this and FakeSMC |
| WhateverGreen  | [Link](https://github.com/acidanthera/WhateverGreen)  | Graphics card injection framework, integrates many patches |

### Others

| Driver Name             | Link                                     | Primary Purpose                                     |
| ---------------- | ---------------------------------------- | ---------------------------------------- |
| AppleBacklightFixup  | [Link](https://bitbucket.org/RehabMan/applebacklightfixup)  | Brightness adjustment driver, already integrated into WhateverGreen v1.2.5  |
| EFICheckDisabler  | [Link](https://github.com/RehabMan/hack-tools/tree/master/kexts/EFICheckDisabler.kext)  | Disables macOS EFI startup check  |
| OS-X-ACPI-Battery-Driver  | [Link](https://bitbucket.org/RehabMan/os-x-acpi-battery-driver) | Battery driver  |
| OS-X-BrcmPatchRAM  | [Link](https://bitbucket.org/RehabMan/os-x-brcmpatchram)  | Broadcom Bluetooth driver  |
| OS-X-EAPD-Codec-Commander  | [Link](https://bitbucket.org/RehabMan/os-x-eapd-codec-commander)  | Fixes sound card sleep mute issue  |
| OS-X-Fake-PCI-ID  | [Link](https://bitbucket.org/RehabMan/os-x-fake-pci-id)  | Hardware ID emulation driver  |
| OS-X-FakeSMC-kozlek  | [Link](https://bitbucket.org/RehabMan/os-x-fakesmc-kozlek)  | SMC emulation driver, choose between this and VirtualSMC  |
| OS-X-Intel-Network  | [Link](https://bitbucket.org/RehabMan/os-x-intel-network)  | Intel wired network card driver (partial)  |
| OS-X-Null-Ethernet  | [Link](https://bitbucket.org/RehabMan/os-x-null-ethernet)  | Emulates wired network card to en0 port, helps connect to Apple Store, etc.  |
<!-- | OS-X-Realtek-Network  |  [Link]([移除了无效网址] -->
