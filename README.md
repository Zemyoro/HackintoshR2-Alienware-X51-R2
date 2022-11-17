# HackintoshR2-Alienware-X51-R2

This repository is meant for Alienware X51 R2 with a Intel Core i7-4790 CPU (Haswell) and Intel AX210 wireless chip.

#### All kexts are updated as of 18 November (2022).

### Note: iMac14,4 release includes kexts supported in Big Sur and below but dropped in Monterey and above

## Important
- Generate SMBIOS with [GenSMBIOS](https://github.com/corpnewt/GenSMBIOS)
- Generate USB map with [USBToolBox Tool](https://github.com/USBToolBox/tool/releases)
- Get macOS online installer from [here](https://dortania.github.io/OpenCore-Install-Guide/installer-guide)
- Get Intel AX210 wireless chip [here](https://www.newegg.com/fenvi-wi-fi6e-mpe-axe3000h-mini-pcie/p/0XM-00JK-000A9)
- Get Intel Core i7-4790 CPU [here](https://www.newegg.com/intel-core-i7-4th-gen-core-i7-4790/p/N82E16819116987)
- Check [here](#change-logs) for change logs

### Software
- SMBIOS model: iMac18,1 (Releases include: iMac16,2 and iMac14,4)
- macOS support: Ventura
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
- USBToolBox: https://github.com/USBToolBox/kext/releases
- WhateverGreen: https://github.com/acidanthera/WhateverGreen/releases (DRM)

### SSDTs
- SSDT-PLUG: https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-PLUG-DRTNIA.aml
- SSDT-EC: https://github.com/dortania/Getting-Started-With-ACPI/blob/master/extra-files/compiled/SSDT-EC-DESKTOP.aml

## Change logs

### v1.0.1
- Debugging/verbose has been disabled

#### To enable:
- Add -v to the beginning of `NVRAM -> Add -> 7C436110-AB2A-4BBB-A880-FE41995C9F82 -> boot-args` value
- Set `Misc -> Debug -> AppleDebug` to `true`
- Set `Misc -> Debug -> Target` to `67`

### v1.0.0
- Most macOS features are supported in this version