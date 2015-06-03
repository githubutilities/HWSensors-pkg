# `pkg` Installer for HWSensors


## Installation

```sh
brew tap githubutilities/tap
brew cask install hwsensors
```


## Uninstallation

```sh
brew cask uninstall hwsensors
brew untap githubutilities/tap
```


## Changes

* Move `ACPISensors.kext`,`CPUSensors.kext`,`GPUSensors.kext`,`LPCSensors.kext` into `FakeSMC.kext` as `PlugIns` for easy management
* `FakeSMC.kext` is installed into `./System/Library/Extensions`
* `HWMonitor.app` is installed into `./Applications`


# Troubleshooting

Use `kextstat | grep FakeSMC` to check its dependencies. Make sure all four plugins(`ACPISensors.kext`,`CPUSensors.kext`,`GPUSensors.kext`,`LPCSensors.kext`) are loaded correctly.


## Original Credits

* [kozlek/HWSensors](https://github.com/kozlek/HWSensors)


## Other FakeSMC Repository

* [RehabMan/OS-X-FakeSMC-kozlek](https://github.com/RehabMan/OS-X-FakeSMC-kozlek)
* [Conti/FakeSMC](https://github.com/Conti/FakeSMC)
