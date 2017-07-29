## TWRP device tree for Kingzone K1 Turbo (K1_turbo)

Add to `.repo/local_manifests/K1_turbo.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/kingzone/K1_turbo" name="android_device_kingzone_K1_turbo" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_K1_turbo-eng
make -j5 recoveryimage
```