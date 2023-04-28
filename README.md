# ShieldOfStamina VR
Simple SKSE plugin making blocking only costs stamina
Does three things:
1. blocking only costs stamina. Health damage is negated at the moment of damage calculation and turned into stamina damaege.
2. when the blocked attack has more damage than the blocker's current stamina is able to handle, the blocker staggers.
3. stifles stamina regen when actor is blocking.

[SE](https://www.nexusmods.com/skyrimspecialedition/mods/62137?tab=posts)
[VR](https://www.nexusmods.com/skyrimspecialedition/mods/90187)

## Requirements
* [CMake](https://cmake.org/)
	* Add this to your `PATH`
* [PowerShell](https://github.com/PowerShell/PowerShell/releases/latest)
* [Vcpkg](https://github.com/microsoft/vcpkg)
	* Add the environment variable `VCPKG_ROOT` with the value as the path to the folder containing vcpkg
* [Visual Studio Community 2022](https://visualstudio.microsoft.com/)
	* Desktop development with C++
* [CommonLibVR](https://github.com/alandtse/CommonLibVR/tree/vr)
	* You need to build from the alandtse/vr branch
	* Add this as as an environment variable `CommonLibVRPath` instead of /extern

## User Requirements
* [VR Address Library for SKSEVR](https://www.nexusmods.com/skyrimspecialedition/mods/58101)
	* Needed for VR

## Register Visual Studio as a Generator
* Open `x64 Native Tools Command Prompt`
* Run `cmake`
* Close the cmd window

### VR
```
cmake --preset vs2022-windows-vcpkg-vr
cmake --build buildvr --config Release
```
## License
[MIT](LICENSE)
