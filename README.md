# Farmeroz's Foundry GURPS Modules

An unofficial collection of modules by Phil Brown (`Farmeroz`) for Foundry Virtual Tabletop and GURPS 4e Game Aid (GGA).

## Install a module

1. Copy the module's **Manifest** link from the table below.
2. In Foundry's **Setup** screen, open **Add-on Modules**.
3. Select **Install Module**, paste the URL into **Manifest URL**, and select **Install**.
4. Enable the module in your world through **Manage Modules**.

Foundry can use the same manifest URL for future updates.  The complete plain-text list is also available in [`manifest-urls.txt`](manifest-urls.txt).

## Module catalogue

Latest stable releases checked on **8 October 2026**.  Versions, compatibility, and dependencies below are taken from the release-tagged manifests; each listed release includes a manifest and module ZIP.  Prereleases are available from individual release pages and are not listed as stable versions.

| Module | Version | Minimum Foundry | Verified Foundry | Requirements | Manifest | Source and releases |
| --- | ---: | ---: | ---: | --- | --- | --- |
| GGA Ammunition & Resource Assistant | 1.2.0 | 13 | 14.367 | GGA 0.18.0+, libWrapper | [Manifest](https://github.com/Farmeroz/gga-ammo-resource-assistant/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-ammo-resource-assistant) · [Releases](https://github.com/Farmeroz/gga-ammo-resource-assistant/releases) |
| GGA Casting Assistant | 0.7.0 | 14 | 14.367 | GGA 0.18.0+, libWrapper | [Manifest](https://github.com/Farmeroz/gga-casting-assistant/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-casting-assistant) · [Releases](https://github.com/Farmeroz/gga-casting-assistant/releases) |
| GGA Expanded Criticals | 0.1.3 | 14 | 14 | GGA 0.18.0+ | [Manifest](https://github.com/Farmeroz/gga-expanded-criticals/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-expanded-criticals) · [Releases](https://github.com/Farmeroz/gga-expanded-criticals/releases) |
| GGA GM Control Sheet | 0.5.0 | 14 | 14.367 | GGA 0.18.0+, libWrapper | [Manifest](https://github.com/Farmeroz/gga-gm-control-sheet/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-gm-control-sheet) · [Releases](https://github.com/Farmeroz/gga-gm-control-sheet/releases) · [Guide](https://github.com/Farmeroz/gga-gm-control-sheet/blob/main/GGA-GM-Control-Sheet-User-Guide.pdf) |
| GGA: GURPS Cone Regions | 0.1.2 | 14 | 14.367 | GGA 0.18.0+ | [Manifest](https://github.com/Farmeroz/gga-gurps-cones/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-gurps-cones) · [Releases](https://github.com/Farmeroz/gga-gurps-cones/releases) |
| GGA Roll Clarity | 0.2.0 | 14 | 14.367 | GGA 0.18.0+ | [Manifest](https://github.com/Farmeroz/gga-roll-clarity/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-roll-clarity) · [Releases](https://github.com/Farmeroz/gga-roll-clarity/releases) |
| GGA Vitality Reserve | 0.1.4 | 14 | 14 | GGA 0.18.23+, libWrapper | [Manifest](https://github.com/Farmeroz/gga-vitality-reserve/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gga-vitality-reserve) · [Releases](https://github.com/Farmeroz/gga-vitality-reserve/releases) · [Guide](https://github.com/Farmeroz/gga-vitality-reserve/blob/main/USER_GUIDE.md) |
| GURPS Action Chases | 0.2.7 | 14 | 14.367 | GGA 0.18.0+ | [Manifest](https://github.com/Farmeroz/gurps-action-chases/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gurps-action-chases) · [Releases](https://github.com/Farmeroz/gurps-action-chases/releases) · [Guide](https://github.com/Farmeroz/gurps-action-chases/blob/main/docs/User-Guide.pdf) |
| GURPS Layered Armour | 0.4.1 | 14 | 14 | GGA 0.18.0+, libWrapper | [Manifest](https://github.com/Farmeroz/gurps-layered-armour/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gurps-layered-armour) · [Releases](https://github.com/Farmeroz/gurps-layered-armour/releases) |
| GURPS Manual Damage | 0.3.2 | 14 | 14 | GGA 0.18.0+ | [Manifest](https://github.com/Farmeroz/gurps-manual-add/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/gurps-manual-add) · [Releases](https://github.com/Farmeroz/gurps-manual-add/releases) |
| Simple Pings | 0.1.0 | 14 | 14 | libWrapper; any game system | [Manifest](https://github.com/Farmeroz/simple-pings/releases/latest/download/module.json) | [Repository](https://github.com/Farmeroz/simple-pings) · [Releases](https://github.com/Farmeroz/simple-pings/releases) |

`modules.json` contains the same stable catalogue, including module descriptions, in a machine-readable form.

## Recent catalogue updates

- **Manual Damage 0.3.2:** fixes the attack-options expander, supports mouse and keyboard activation, and preserves its state after area changes.
- **Foundry v14 verification:** Manual Damage 0.3.2, Expanded Criticals 0.1.3, Vitality Reserve 0.1.4, and Layered Armour 0.4.1 now explicitly declare verified v14 compatibility.

- **Ammunition & Resource Assistant 1.2.0:** optional GURPS 4e malfunctions, outcome-aware ammunition spending, persistent weapon condition, and clearing/repair records, alongside guided bow and throwing actions.
- **Layered Armour 0.4.0:** layered GURPS 4e protection plus optional Basic Set and Shields Up! shield damage, visible condition trackers, repairs, undo, and residual damage review.
- **Manual Damage 0.3.1:** damage entry and rolls, fragmentation resolution, and review through GGA's native Apply Damage Dialog.

## Legacy module

[**UI UI no UI 1.0.0**](https://github.com/Farmeroz/ui-ui-no-ui/releases/tag/ui-ui-no-ui) is Farmeroz's published copy of Boifubá's UI visibility module.  Its release notes describe toggling UI elements in GGA with **Ctrl+H**.  The tagged manifest declares Foundry 12 minimum and Foundry 13 verified; it still contains placeholder `my-user` manifest and download URLs.  It is therefore listed here for completeness, rather than in the stable installation list.  Foundry 14 compatibility has not been established by that manifest.

## Support

Use the **Issues** tab in the relevant module repository to report a problem or request an enhancement.  Include the Foundry, GGA, and module versions and any console error messages.

Simple Pings is released under LGPL v3, preserving the original Pings licence and attribution.  The other modules are released under the MIT licence in their own repositories.

GURPS is a trademark of Steve Jackson Games.  These unofficial modules are not affiliated with or endorsed by Steve Jackson Games, Foundry Gaming LLC, or the GURPS Game Aid maintainers.
