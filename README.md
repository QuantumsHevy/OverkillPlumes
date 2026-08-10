# Overkill Plumes

Switchable configurations for some engines that aim for stylistic and somewhat hard-sci-fi-accurate exhaust plumes. Mainly just ModuleManager patches and homemade Waterfall templates.

![A distant shot of the Niven's plume burning low-throttle near Jinzha.](Media/niven_helltaker_distant.png)

## Dependencies

These mods are **required** for Overkill Plumes to run properly. You'll need to install each one (and their own dependencies) before installing Overkill in order for it to work.

- [Waterfall](https://github.com/KSPModStewards/Waterfall)
  - The Waterfall effects framework is used to render custom engine plumes.
- [ModuleManager](https://github.com/sarbian/ModuleManager)
  - Effects are applied to parts using ModuleManager patches.
- [B9PartSwitch](https://github.com/blowfishpro/B9PartSwitch)
  - In-game plume switches are created using B9PartSwitch modules.

## Compatibilities
These mods are **not required** for Overkill to run, but are currently supported through patches. Effectively, these are mods whose engines can get Overkill plumes. 

- [Far Future Technologies](https://github.com/post-kerbin-mining-corporation/FarFutureTechnologies)
  - X-2 'Heinlein' Nuclear Salt Water Rocket Engine
  - x-42 'Niven' Nuclear Salt Water Rocket Engine
  - A-834M 'Frisbee' Antimatter Torch Engine (Compatible with [Interstellar Plumes](https://spacedock.info/mod/4110/Interstellar%20Plumes))

- [Stock Waterfall Effects](https://github.com/KnightofStJohn/StockWaterfallEffects)
  - LV-N 'Nerv' Atomic Rocket Motor (Compatible with [Restock](https://github.com/PorktoberRevolution/ReStocked))
  - Kerbodyne KR-2L+ 'Rhino' Liquid Fuel Engine (Compatible with [Restock](https://github.com/PorktoberRevolution/ReStocked))

Every supported engine gets a plume switcher in their right-click menus. Most switchers also offer a faux-antimatter option for that little asthetic kick, alongside the Overkill and original plumes.

![A shot of the Heinlein's plume on the MITOS SS530 New Haven, burning full-throttle in low orbit of Eve.](Media/heinlein_new-haven.png)

![The MITOS SS557X Helltaker burning full throttle near Yunxaio.](Media/niven_helltaker_full-throttle.png)

## Installation

### via CKAN
A CKAN listing is actively being worked on. [Download via the SpaceDock link below](#via-spacedockgithub) for the latest actual release.
<!--
Search for "Overkill Plumes" in your CKAN client and install the mod as usual. CKAN will also flag any dependencies and install those as well.
-->
```
depends:
  - name: Waterfall
  - name: ModuleManager
  - name: B9PartSwitch
reccomends:
  - name: FarFutureTechnologies
  - name: StockWaterfallEffects
suggests:
  - name: Restock
  - name: RestockPlus
conflicts:
  - name: KerbalAtomics
```

### via SpaceDock/GitHub
Download the latest ZIP from [SpaceDock](https://spacedock.info/mod/4447/Overkill%20Plumes) (or [the GitHub repo's Releases page](https://github.com/QuantumsHevy/OverkillPlumes/releases)), extract it, and drag ONLY the `OverkillPlumes` folder inside your KSP installation's `GameData` folder. You can also simply extract the ZIP file directly into `GameData` using File Explorer's "Extract all" option.

When done correctly, the path should look like this:
```
KerbalSpaceProgram/
└── GameData/
    ├── OverkillPlumes/
    │   ├── FX/
    │   ├── Patches/
    │   └── ...
    ├── Squad/
    ├── YourOtherMods/
    └── ...
```

## Known Issues

- Overkill plumes don't react to atmosphere depth and only ever display vaccum-accurate plumes. This is intentional for the first few releases, and atmosphere-accurate plumes will be added to all supported engines over the span of future updates.
- When ReStock is installed, the throttle response rates for the Nerv and Rhino are repeatedly set to comparatively low values. This is because of a patch order that rebuilds SWE's Waterfall modules after all of Overkill's edits, and they cannot reliably be overwritten again without employing some questionable ModuleManager practices. A fix is shelved for now.
- **KerbalAtomics conflicts with Overkill Plumes.** Installing it alongside Restock and SWE causes the Nerv's LF mode to lose its sound and visible plume. This is a conflict between KerbalAtomics' and Restock's own patches, and is outside of Overkill's scope to fix.

## Credits

- **[Quantums Hevy](https://github.com/QuantumsHevy)**, original mod author

![A detailed close-up of the Helltaker burning full throttle near Jinzha.](Media/niven_helltaker_close.png)

## License

Copyright © 2026 Quantums Hevy

This work is licensed under the [GNU General Public License v3.0.](./COPYING) (GPL-3.0). 

This project contains patches and configuration files intended for use with other third-party Kerbal Space Program mods. No ownership of those other projects or their assets is claimed, and nothing in this repository alters or supersedes their respective licenses.
