<p align="center">
  <img src="https://i.imgur.com/lyJkVeK.png"/>
</p>

We aim to bring a more consistent, fluent and smooth experience with all your must-have customizations, for you, for the community, and for everyone.

# Build guide

Prior to building, you will need basic knowledge of [Git](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet).

### Requirements
- Around 100G disk space.
- A computer with at least 16GB RAM running Linux (recommended) or MacOS.
- Build environment [setup](https://github.com/akhilnarang/scripts).

### Instructions
1. Run the following commands to sync source

```
repo init -u https://github.com/Project-Awaken/android_manifest -b triton
```
2. To sync source, enter

```
 repo sync -c --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all)
```

3. Once the source is downloaded/synced, prepare your device trees, dependencies and start the build by the following commands

```
   source build/envsetup.sh
   lunch awaken_<devicecodename>-user
   make bacon -j$(nproc --all)
```

### Compilation Help
To get help with build errors, please visit [**Android Building Help**](https://t.me/AndroidBuildingHelp).

## Credits

 * [**LineageOS**](https://github.com/LineageOS)
 * [**CodeAurora Forum**](https://source.codeaurora.org/quic/la)
 * [**ArrowOS**](https://github.com/ArrowOS)
 * [**Project-Fluid**](https://github.com/Project-Fluid)
 * [**ProtonAOSP**](https://github.com/ProtonAOSP)
 * [**PixelExperience**](https://github.com/PixelExperience)
 * [**ABC-ROM**](https://github.com/ezio84)
 * [**AospExtended**](https://github.com/AospExtended)
 * [**Syberia Project**](https://github.com/syberia-project)
 * [**Yet another AOSP project**](https://github.com/Yaap)
 * [**Krypton Open Source Project**](https://github.com/Aosp-Krypton)

# Maintainership

### Requirements
You don't need a lot of skills to be a device maintainer. You only need to have:
- enough git skills to properly handle your device specific repos, and
- the ability to read logs, so you can know any device related issues and fix them.

To apply for official status, please fill the maintainership application [**form**](https://github.com/Project-Awaken/official_devices).

### Links to official groups/channels
- [**Discussion Group**](https://t.me/AwakenOSChat)
- [**Announcements Channel**](https://t.me/AwakenOSNews)
- [**Updates Channel**](https://t.me/AwakenOSUpdates)
