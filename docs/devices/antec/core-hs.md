title: Antec Core HS

<style>
  code {white-space: nowrap;}
  kbd {white-space: nowrap;}
  no-wrap {white-space: nowrap;}
</style>

# Antec Core HS

![](../../_inc/images/devices/ayaneo-slide.png){ .off-glb }

!!! warning
    This device is currently unsponsored.
    Information may be out of date or incorrect.

!!!info
    New AMD 7000 series devices do not support S3 sleep and must be configured for Modern Standby + s0i3.
    Follow the [process on the Wiki](https://wiki.steamfork.org/troubleshooting/#enabling-modern-sleep-on-7000-series-amd-based-devices) to configure your device.

## Features

| Feature | Notes |
| -- | -- |
| <no-wrap>:material-harddisk: Storage</no-wrap> | SteamFork can be run from a USB Drive or installed directly to the internal NVME. 
| <no-wrap>:material-wifi: Wifi</no-wrap> | Can be turned on in Steam OS under `Main Menu` > `Network Settings`. |
| <no-wrap>:simple-bluetooth: Bluetooth</no-wrap> | Supports bluetooth audio and controllers. |
| <no-wrap>:material-fan: Fan</no-wrap> | Controlled by system firmware. |
| <no-wrap>:material-lightning-bolt-circle: TDP Limit</no-wrap> | Can be set globally, per system or per game. Requires the [SimpleDeckyTDP](https://github.com/SteamFork/SimpleDeckyTDP) plugin.|
| <no-wrap>:material-vibrate: Rumble</no-wrap> | Enables the device rumble motor in emulators that support it. |
| <no-wrap>:material-lightbulb-on: RGB</no-wrap> | Disabled on startup. Requires the [HueSync](https://github.com/honjow/HueSync) plugin for additional RGB control.|

### Function Buttons

| Button | Function |
| -- | -- |
| ++"Aya"++ | <kbd>:material-microsoft-xbox: Guide</kbd> <no-wrap>(`Steam Menu`)</no-wrap> |
| <kbd>:material-equal:</kbd> | <no-wrap><kbd>:material-microsoft-xbox: Guide</kbd> + <kbd>:material-gamepad-circle-down: A</kbd></no-wrap> <no-wrap>(`Quick Access Menu`)</no-wrap> |
| ++"LC"++ | ++"L4"++ |
| ++"RC"++ | ++"R4"++ |

## Notes

### Installation

Download the latest `AMD64` version of SteamFork from the button below and follow the instructions listed on the [Install](../../../play/install/) page.

[![Latest Version](https://img.shields.io/github/release/SteamFork/distribution.svg?labelColor=111111&color=5998FF&label=Latest&style=flat#only-light)](https://github.com/SteamFork/distribution/releases/latest)
[![Latest Version](https://img.shields.io/github/release/SteamFork/distribution.svg?labelColor=dddddd&color=5998FF&label=Latest&style=flat#only-dark)](https://github.com/SteamFork/distribution/releases/latest)

### Known Issues

* An unknown issue exists that causes the device to reboot unexpectedly.  There is no notification or panic log.
* When Modern Standby is enabled, the power button does not send events to the OS.  Sleep works with Modern Standby + Si02 when selected from the Steam interface.

### Booting from an external drive (USB or SD Card)

To boot SteamFork from an external drive, hold <no-wrap>++"LC"++ + <kbd>:material-plus: Volume Up</kbd></no-wrap> and press <kbd>:material-power: Power</kbd> ,
continue holding <no-wrap>++"LC"++ + <kbd>:material-plus: Volume Up</kbd></no-wrap> until the Ayaneo logo appears.
Select the storage device with SteamFork from the boot menu using the ++"Ayaneo"++ button, and then press <kbd>:material-plus: Volume Up</kbd> to boot the distribution.
