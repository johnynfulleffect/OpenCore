# Hardware

CPU: AMD Ryzen 5 3600 6-Core 4.2Ghz

GPU: Radeon RX Vega 56 8GB RAM

RAM: Kingston HyperX Fury 16GB DDR 3466Mhz

Motherboard: ASUS ROG Strix 450-I AM4

Audio Codec: AppleALM Profile 7

Ethernet Card: Intel I211-AT Gigabit

Wifi/BT Card: BCM94360CS2 + NGFF M.2 Key A/E Adapter

BIOS revision: 3004


# Guide

[OpenCore Desktop Guide](https://dortania.github.io/OpenCore-Desktop-Guide/AMD/zen.html#ryzen-and-threadripper17h)

# Key Updates

- The ROG BIOS has no option for the above 4G decoding so I had to disable `IncreasePciBarSize` in the Kernal : Quirks
- Add `npci=0x2000` to NVRAM : Add : boot-args.
- Add `alcid: 7` to NVRAM : Add : boot-args.

Followed the recommended BIOS settings as well as added the HPET ACPI and patches.
