# HackintoshR2-Alienware-X51-R2

This repository is meant for Alienware X51 R2 with a Intel Core i7-4790 CPU (Haswell) and Intel AX210 wireless chip. Check [here](#change-logs) for change logs.

#### All kexts are updated as of 17 November (2022). Generate SMBIOS with [this repository](https://github.com/corpnewt/GenSMBIOS).

### Software
- SMBIOS model: iMac16,2
- macOS support: Monterey
- OpenCore version: 0.8.6

### Hardware
- CPU: Intel Core i7-4790 (Haswell)
- Wireless: Intel AX210
- Ethernet: Realtek RTL8111

### Drivers
- HFSPlus: https://github.com/acidanthera/OcBinaryData/blob/master/Drivers/HfsPlus.efi
- OpenRuntime: https://github.com/acidanthera/OpenCorePkg/releases (In drivers by default)

### Kexts
- AirPortItlwm: https://github.com/OpenIntelWireless/itlwm/releases (Wi-Fi, Find My, AirDrop, AirPlay, Handoff, etc.)
- AppleALC: https://github.com/acidanthera/AppleALC/releases (Audio)
- BlueToolFixup: https://github.com/acidanthera/BrcmPatchRAM/releases (Bluetooth)
- FeatureUnlock: https://github.com/acidanthera/FeatureUnlock/releases (Sidecar, Airplay to Mac, etc.)
- IntelBluetoothFirmware: https://github.com/OpenIntelWireless/IntelBluetoothFirmware/releases (with IntelBTPatcher) (Bluetooth)
- Lilu: https://github.com/acidanthera/Lilu/releases (Kext patcher)
- RealtekRTL8111: https://github.com/Mieze/RTL8111_driver_for_OS_X/releases (Ethernet)
- VirtualSMC: https://github.com/acidanthera/VirtualSMC/releases (Apple SMC Emulator)
- USBToolBox: https://github.com/USBToolBox/kext/releases (https://github.com/USBToolBox/tool/releases for generating your own UTBMap kext)
- WhateverGreen: https://github.com/acidanthera/WhateverGreen/releases (DRM)

### SSDTs
- SSDT-PLUG: https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PLUG-DRTNIA.aml
- SSDT-EC: https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-DESKTOP.aml

## Change logs

### v1.0.0
- Most macOS features are supported in this version