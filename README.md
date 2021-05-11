# HP-EliteDesk-800-G5-DM-with-OpenCore

Here attached the content of the EFI partition

### Status: Running

Currently running:

| Component     | Version      |
| ------------- | ------------ |
| macOS version | 11.3.1 (20E241 |
| OpenCore      | 0.6.9        |
| BIOS version  | Q21 Ver. 02.15.00        |

## Hardware info

| Component | Model                                   |
| --------- | --------------------------------------- |
| CPU       | Intel(R) Core(TM) i7-8700    |
| Memory    | 32GB                       |
| Storage   | WDC PC SN520 SDAPNUW-512G-1006                 |
| Display   | HP E24D G4 (through DP)                 |
| GPU       | Intel UHD Graphics 630 (Desktop)                          |
| WLAN      | BCM4352 (replacement of original WIFI Card / eBay) |

## Status

### Working

- [x] Keyboard (external through USB)
- [x] Audio (AppleALC)
- [x] Ethernet
- [x] Bluetooth
- [x] Sleep/wake
- [x] Mouse (external through USB)

## Compatible BIOS settings

| Parameter     | Value      |
| ------------- | ------------ |
| TPM Device | Hidden |
| TPM State | Disable |
| TPM Activation Policy | No prompts |
| Fast Boot | Disable |
| Network (PXE) Boot | Disable |
| Configure Legacy Support and Secure Boot | Legacy Support Disable and Secure Boot Disable |
| HP Application Driver | Disable |
| Wake On LAN | Disabled |
| Extended Idle Power States | Enable |
| Video Memory Size | 64 MB |
| Intel Software Guard Extensions (SGX) | Disable |
| Virtualization Technology (VTx) | Disable |
| Virtualization Technology for Directed I/O (VTd) | Disable |
| Trusted Execution Technology (TXT) | Disable | 
  
## Post-install

sudo pmset autopoweroff 0
sudo pmset powernap 0
sudo pmset standby 0
sudo pmset proximitywake 0
sudo pmset tcpkeepalive 0

## CREDITS

- [Acidanthera](https://github.com/acidanthera)
- [Dortania OC guide](https://dortania.github.io/OpenCore-Install-Guide/)
- [Rehabman's battery patch guide](https://www.tonymacx86.com/threads/guide-how-to-patch-dsdt-for-working-battery-status.116102/) and [Rehabman's ACPI hotpatching guide](https://www.tonymacx86.com/threads/guide-using-clover-to-hotpatch-acpi.200137/)
- [OpenWireless and itlwm](https://github.com/OpenIntelWireless/itlwm)
- Thanks also to Hackintool / great tool
- Thanks also to OpenCore Configurator / great tool too :)
