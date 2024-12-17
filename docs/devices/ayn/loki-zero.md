# Loki Zero

![](../../_inc/images/devices/ayn-loki.png){ .off-glb }

!!! warning
    This device is currently unsponsored.
    Information may be out of date or incorrect.

## Features

| Feature&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Notes |
| -- | -- |
| :material-harddisk: Storage | SteamFork can be run from an SD Card, USB Drive or installed directly to the internal NVME. |
| :material-wifi: Wifi | Can be turned on in Steam OS under Main Menu > Network Settings. |
| :simple-bluetooth: Bluetooth | Supports bluetooth audio and controllers. |
| :material-fan: Fan | Managed automatically. |
| :material-lightning-bolt-circle: TDP Limit | Can be set globally, per system or per game. Requires the [SimpleDeckyTDP](https://github.com/SteamFork/SimpleDeckyTDP) plugin.|
| :material-vibrate: Rumble | Enables the device rumble motor in emulators that support it. |
| :material-lightbulb-on: RGB |Disabled on startup. Requires the [HueSync](https://github.com/honjow/HueSync) plugin for additional RGB control.|

## Notes

### Installation

Download the latest `AMD64` version of SteamFork from the button below and follow the instructions listed on the [Install](../../../play/install/) page.

[![Latest Version](https://img.shields.io/github/release/SteamFork/distribution.svg?labelColor=111111&color=5998FF&label=Latest&style=flat#only-light)](https://github.com/SteamFork/distribution/releases/latest)
[![Latest Version](https://img.shields.io/github/release/SteamFork/distribution.svg?labelColor=dddddd&color=5998FF&label=Latest&style=flat#only-dark)](https://github.com/SteamFork/distribution/releases/latest)

### Booting from an external drive (USB or SD Card)

In order to launch SteamFork from an external drive you will need to first change the boot order in the BIOS.  

During boot you can enter the bios by either (1) holding the ++"Home"+"LCC (Turbo)"++ buttons that sit bellow the dpad and right analog stick OR (2) connecting an external keyboard and pressing the ++del++ key.  

In the bios; navigate to the `Boot` menu and then change the boot order to prioritize the SD card or USB Drive under `Boot Order Priorities`. Then go `Save & Exit` and select the Save Changes and Exit option.  This change will persist through all reboots.  If you want to boot into Windows simply remove the SD Card or USB drive.
