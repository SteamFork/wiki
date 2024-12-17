title: MSI Claw A1M

<style>
  code {white-space: nowrap;}
  kbd {white-space: nowrap;}
  no-wrap {white-space: nowrap;}
</style>

# MSI Claw A1M

![](../../_inc/images/devices/msi-claw.png){ .off-glb }

!!! warning
    This device is currently unsponsored.
    Information may be out of date or incorrect.

## Features

| Feature | Notes |
| -- | -- |
| <no-wrap>:material-harddisk: Storage</no-wrap> | SteamFork can be run from an SD Card, USB Drive or installed directly to the internal NVME. <br> When installed directly to the NVME; an SD Card can be used for game storage. |
| <no-wrap>:material-wifi: Wifi</no-wrap> | Can be turned on in Steam OS under Main Menu > Network. |
| <no-wrap>:simple-bluetooth: Bluetooth</no-wrap> | Supports bluetooth audio and controllers. |
| <no-wrap>:material-fan: Fan</no-wrap> | Controlled by system firmware. |
| <no-wrap>:material-lightning-bolt-circle: TDP Limit</no-wrap> | Can be set globally, per system or per game. Requires the [SimpleDeckyTDP](https://github.com/SteamFork/SimpleDeckyTDP) plugin. |
| <no-wrap>:material-vibrate: Rumble</no-wrap> | Enables the device rumble motor in software that supports it. |

### Function Buttons

| Button | Function |
| -- | -- |
| ++"MSI Center"++ | <kbd>:material-microsoft-xbox: Guide</kbd> <no-wrap>(`Steam Menu`)</no-wrap> |
| ++"Quick Settings"++ | <no-wrap><kbd>:material-microsoft-xbox: Guide</kbd> + <kbd>:material-gamepad-circle-down: A</kbd></no-wrap> <no-wrap>(`Quick Access Menu`)</no-wrap> |

## Notes

### Installation

Download the latest `AMD64` version of SteamFork from the button below and follow the instructions listed on the [Install](../../../play/install/) page.

[![Latest Version](https://img.shields.io/github/release/SteamFork/distribution.svg?labelColor=111111&color=5998FF&label=Latest&style=flat#only-light)](https://github.com/SteamFork/distribution/releases/latest)
[![Latest Version](https://img.shields.io/github/release/SteamFork/distribution.svg?labelColor=dddddd&color=5998FF&label=Latest&style=flat#only-dark)](https://github.com/SteamFork/distribution/releases/latest)

### Known Issues

* Sleep currently does not work properly.  Attempting to sleep will break some controls until the device is powered off with external power removed.
* WiFi performance can be erratic at times.
* Sound occasionally becomes glitchy or stops working altogether until the device is rebooted.
* Sound currently does not work over HDMI.
* Game support is currently hit-or-miss.  DirectX 12 may be especially problematic.
* Built-in controls currently cannot be recalibrated.
* Paddle buttons currently cannot be remapped.
* RGB currently cannot be controlled.
* Mangohud does not display CPU or GPU power draw and does not correctly display GPU usage.

### Booting from an external USB drive (USB or SD Card)

In order to boot SteamFork, `Secure Boot` will need to be disabled.

Power on the device and hold <no-wrap>++"RB"+"RT"++</no-wrap> until the BIOS appears.
Using the <kbd>:material-gamepad-round: D-pad</kbd> and <kbd>:material-gamepad-circle-down: A</kbd> or the touchscreen,
navigate to `Security`, select `Secure Boot`, `Secure Boot Support` and select `Disabled`.
Afterwards, navigate to `Save & Exit` and select `Save Changes and Reset`.

Once Secure Boot is disabled, power on the device and hold <no-wrap>++"LB"+"RB"++</no-wrap> until the Boot Menu appears.
Using the <kbd>:material-gamepad-round: D-pad</kbd> and <kbd>:material-gamepad-circle-down: A</kbd> or the touchscreen, select the storage device with SteamFork to boot the distribution.
