# Hardware

CPU: AMD Ryzen 5 3600 6-Core 4.2Ghz

GPU: Radeon RX Vega 56 8GB RAM

RAM: Kingston HyperX Fury 16GB DDR 3466Mhz

Motherboard: ASUS ROG Strix B450-I AM4

Audio Codec: AppleALM Profile 7

Ethernet Card: Intel I211-AT Gigabit

Wifi/BT Card: BCM94360CS2 + NGFF M.2 Key A/E Adapter

BIOS revision: 4202


# Guide

[OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Install-Guide/AMD/zen.html#starting-point)

[Fixing Audio](https://dortania.github.io/OpenCore-Post-Install/universal/audio.html#fixing-audio-with-applealc)


# Key Updates

- The BIOS has no option for the above 4G decoding so I had to disable `IncreasePciBarSize` in the Kernal : Quirks
- Add `npci=0x2000` to NVRAM : Add : boot-args.
- Add `alcid: 7` to NVRAM : Add : boot-args.
- Run HPET option in SSDTTime and add ACPI and patches.

# BIOS Changes

- Disabled Fast Boot
- In Secure Boot, set to Windows UEFI Mode
- Disabled CSM
- Enabled EHCI/XHCI Hand-off

# Third Party Fixes

- Adobe Photoshop was quitting upon load.  Ran PS2020 script here: [AdobeFixAMD](https://gist.github.com/XLNCs/86d7a391e46f85a04d28db171656b458)
