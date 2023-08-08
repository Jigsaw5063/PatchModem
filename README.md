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
- Properly loads MBN back, when the network connection is poor/dropped

## Verified
- LG V60, ATT - Mexico City > 5G - VoLTE & VoWiFi
- Pixel 5 - Orange Romania - VoLTE & VoWiFi & 5G
- Pixel 5 - Orange T-Mobile - VoLTE & VoWiFi

## Difference between this module and ender-zhao module
- Doesn't enforce 5G
- After loosing connection to the network provider the original module didn't load MBN back again. We had to restart Pixel5

# Credits
- Big thanks to [mightyvenom](https://forum.xda-developers.com/m/mightyvenom.4163960/) from XDA with testing module and feedback
- Big thanks to ender-zhao for providing initial Magisk Module

# QPST/EFS Method
There's a old method with loading MBNs directly to the MODEM NV in folder `QPST EFS Method`
You can use it if this module doesn't work and you have proper MBN.
