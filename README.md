# Intel NUC8i5BEH (Comet Lake) - macOS 12

<p align="center">
    <img height="auto" width="auto" src="images/screenshot.png" />
</p>

## OpenCore configuration for macOS Monterey

**For educational purposes**. I don't take any responsibility for you voilating the Apple ToS and/or damaging your device.

## Installation

```
PlatformInfo -> Generic -> Add Serial, SystemUUID and MLB for SMBIOS Macmini8,1
```

## Base Specs

- CPU: i5-8259U
- GPU: HD655
- Audio Codec: ALC235
- Model: NUC8i5BEH
- Mobo: NUC8BEB
- Ethernet: Intel I219-V
- Wifi & Bluetooth: Intel AC 9560

## BIOS

Update to v088 [here](https://downloadcenter.intel.com/download/30430/BIOS-Update-BECFL357-)

```md
Devices -> USB -> Port Device Charging Mode: off
Devices -> USB -> USB Legacy -> Disabled
Security -> Thunderbolt Security Level: Legacy Mode
Power -> Wake on LAN from S4/S5: Stay Off
Boot -> Boot Configuration -> Network Boot: Disable
Boot -> Secure Boot -> Disable
```

## Notes

Everything is working except Thunderbolt Hot-Plug.

Intel WiFi + Bluetooth is working stable for me. WiFi will be shown as Ethernet Interface, thus GUI switching requires custom client [HeliPort](https://github.com/OpenIntelWireless/HeliPort).

## Test Devices

- WiFi
  - Telekom Speedport Smart
  - Xiaomi AC2100
- Bluetooth
  - Logitech MX Master 3 Mac
  - Keychron K3
- Thunderbolt
  - LG 34UC99-W

## Credits

- [Nucintosh](https://github.com/zearp/Nucintosh)
