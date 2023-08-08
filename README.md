# PatchModem after croosflash to EU firmware.

## Introduction
This module enables VoLTE & VoWiFi & 5G in unsupported carriers worldwide :)

Enable Network and Mobile Data after croosflash to EU firmware.

Added MBNs for many regions but not sure if it will work properly as it is not signed with LG certificate.
Check MBNs in the folder: `/system/vendor/firmware_mnt/image/modem_pr/mcfg/configs/mcfg_sw/generic/` in this repo, if you want to see if your country is available within this module.
This module designed for the LG V60, but it should work for other models as well.


## Usage - How to use
1. Download latest version from [Release page](https://github.com/stanislawrogasik/Pixel5-VoLTE-VoWiFi/releases)
2. Flash in Magisk
3. Reboot & enjoy 

## Features
- **Doesn't enforce 5G** - you can still select LTE only if your current provider plan doesn't support 5G
- Enables VoLTE
- Enables VoWiFi
- Enables 5G support
- Added more MBN for carriers, i am not sure will it work because we have to LG certificed MBNs.

## Verified
- LG V60, ATT - Mexico City > 5G - VoLTE & VoWiFi
- LG V60, ATT - Orange Romania - VoLTE & VoWiFi & 5G
- LG V60, ATT - Orange T-Mobile - VoLTE & VoWiFi

# Patched modem images
- If you don't have root you can use [Patched Modem image](https://forum.xda-developers.com/t/modem-patched-or-pdc-tool-fixed-lte-mobile-data.4537979/) also you can comment there for your feedback.
- 

# QPST/EFS Method or via PDC tool
There's a  method with loading MBNs directly to the MODEM NV in folder `QPST EFS Method` or Load via PDC tool.
You can use it if this module or image doesn't work and you have proper MBN.
