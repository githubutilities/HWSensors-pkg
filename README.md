# `pkg` Installer for HWSensors


## Changes

* Move `ACPISensors.kext`,`CPUSensors.kext`,`GPUSensors.kext`,`LPCSensors.kext` into `FakeSMC.kext` as `PlugIns` for easy management
* `FakeSMC.kext` is installed into `./System/Library/Extensions`
* `HWMonitor.app` is installed into `./Applications`


## Original Credits

* [kozlek/HWSensors](https://github.com/kozlek/HWSensors)

