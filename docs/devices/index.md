title: Device Support

# :material-television: Device Support

## Tested devices

SteamFork has been tested (i.e. booted at least once) on the list of devices below marked sponsored and verified.  Devices with a sponsor are actively tested and used with SteamFork frequently.  Devices without a sponsor are not actively tested by a dedicated maintainer and may have unknown issues. While untested, modern laptops, desktops, and mini PCs with Intel or AMD should not have any issues.

| Manufacturer | Product | Sponsor <sup>1</sup> |
| -- | -- | -- |
| Anbernic | [Win600](anbernic/win600) | Community Verified |
| ANTEC | [Core HS](antec/core-hs.md) <sup>2</sup> | Community Verified |
| ASUS | [ROG Ally / Ally X](asus/rog-ally) | [flukejones](https://github.com/flukejones) |
| Atari | [VCS](atari/vcs.md) | Community Verified |
| AYANEO | [2](ayaneo/ayaneo-2) | Community Verified |
| AYANEO | [2S](ayaneo/ayaneo-2s) <sup>3</sup> | [Fewtarius](https://github.com/fewtarius) |
| AYANEO | [Air / Air Pro](ayaneo/air.md) | Community Verified |
| AYANEO | [Air 1S](ayaneo/air-1s) <sup>3</sup> | [winghugs](https://github.com/winghugs) |
| AYANEO | [Air Plus (AMD 6800U)](ayaneo/air-plus-6800u) | [uejji](https://github.com/uejji) |
| AYANEO | [Flip KB](ayaneo/flip-kb) <sup>2</sup> | [Fewtarius](https://github.com/fewtarius) |
| AYANEO | Geek | Community Verified by [alexapple79](https://www.youtube.com/watch?v=4iBE-PUC_0Y) |
| AYANEO | Next, Next Lite, Next Pro | Community Verified |
| AYANEO | [Slide](ayaneo/slide.md) <sup>2</sup> | Community Verified |
| AYN | [Loki Max](ayn/loki-max) | [Fewtarius](https://github.com/fewtarius) |
| AYN | [Loki Zero](ayn/loki-zero) | Community Verified |
| GPD | [Win 4 (AMD 6800U)](gpd/win4-6800u) | [anthonycaccese](https://github.com/anthonycaccese) |
| GPD | Win 4 (AMD 7840U) | Community Verified by [Maeiourk](https://github.com/maeiourk) |
| GPD | Win Mini | Community Verified |
| MSI | [Claw A1M](msi/claw-a1m) | Community Verified |

!!! info
    1. Sponsored devices are fully supported by its maintainer.  Support for unsponsored and community verified devices may vary.
    2. Some AMD 7000 series devices do not support S3 sleep and must be configured for Modern Standby + s0i3.  This setting is locked down on many Ayaneo devices and must be enabled using a third party helper.  Follow the [process on the Wiki](https://wiki.steamfork.org/troubleshooting/#enabling-modern-sleep-on-7000-series-amd-based-devices) to configure your device.
    3. Requires a BIOS update for modern sleep to work correctly.
    4. Support for these devices is still a work in progress. Expect bugs or incomplete/missing features as support is being added. Refer to the specific device's page for more information.

## Sponsoring a device

### Sponsorship
Sponsoring a device is a commitment to maintaining support for your device by validating, testing, and bugfixing any issues that may arise.  Adding support for a device's basic features is straight forward, however, it can become far more technical to add support for features such as fan control.  If you are interested in sponsoring your device, follow the process below.

1. Create a GitHub account if you do not already have one.
2. Boot the SteamFork installation image.
3. Create a device quirk using the [quirk creation tool](https://wiki.steamfork.org/contribute/quirks/) included with the distribution.  Minimum requirements are gamescope resolution, and rotation if needed.
4. Create a pull request to the [SteamFork Device Support](https://github.com/SteamFork/distribution/tree/main/PKGBUILD/steamfork-device-support) package with your new addition.
5. Open and take ownership of any issues specific to your device on [discord](https://github.com/SteamFork#community).
6. When ready to begin sunsetting support for your device, generate and PR new quirk with the `--supported false` property.
