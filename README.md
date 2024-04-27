## Recovery Device Tree for the 2019 Samsung Galaxy Tab A [SM-T510]

## How-to compile it:


To initialize your local repository using the AOSP trees to build TWRP, use a command like this:

```sh
repo init --depth=1 -u git://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-11
```
Then to sync up:

```sh
repo sync
```
Then to build:

```sh
export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch twrp_gta3xlwifi-eng; mka recoveryimage

```

All credit goes to Magendanz, for getting the ball rolling on the builds. His TWRP builds are base to all available variants to lineage of it. Treble-based roms, and more. So cheers to C.M. 

I own the SM-T510 so I have an interest in continuing development. Moving it along, much as the hardware itself will allow. 

For reference, this is his recovery device tree which started it all. Not necessarily up to date with his latest 3.7 TWRP build (available via XDA), but valuable nonetheless. Used it as a starting point for my builds.
