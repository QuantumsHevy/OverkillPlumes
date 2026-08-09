# Changelog
All notable user-facing changes to Overkill Plumes are documented in this file. This mod is compatible with Kerbal Space Program 1.12 unless noted otherwise. Version numbers should follow semantic versioning.

## v0.2.0
### Added
- Added a plume switcher to every supported engine. Right-click the engine in the VAB/SPH (or in flight) to choose between the Overkill exhaust and the original plume.
- Added an Overkill plume for the LV-N 'Nerv' Atomic Rocket Motor, including a ReStock-aware variant.
- Added an Overkill plume for the Kerbodyne KR-2L+ 'Rhino' Liquid Fuel Engine, including a ReStock-aware variant.
- Added an Overkill plume for FFT's A-834M 'Frisbee' Antimatter Torch Engine, including an extra "Venture Star" plume option if Interstellar Plumes is also installed.
- Added a bit of original MITOS in-universe lore to several plume descriptions.
### Changed
- Waterfall, ModuleManager, and B9PartSwitch are now Overkill's core dependencies. Stock Waterfall Effects and Far Future Technologies are compatibility layers instead; SWE unlocks the stock Nerv and Rhino plumes, and FFT unlocks its own NSWR and Frisbee plumes.
### Issues
- KerbalAtomics conflicts with Overkill when ReStock is also installed. The stock Nerv's LF mode loses its sound and visible plume despite functioning thrust. See the README's Known Issues section for details.
- Installing ReStock causes SWE's patches to reapply after Overkill's on the Nerv and Rhino, resetting Overkill's throttle response-rate tuning back to default. The plume itself still displays and switches correctly.

## v0.1.0
### Added
- Added (vacuum only) Overkill plumes for the X-42 'Niven' and the X-2 'Heinlein' NSWR Engines.
<!--
### Fixed
- 
### Added
- 
### Changed
- 
### Issues
- 
-->