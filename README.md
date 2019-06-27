## TWRP device tree for Turkcell T70 (P809T70) Zte Blade A506 (P809F52)

Add to `.repo/local_manifests/P809T70.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project name="nightslex/android_device_zte_P809T70-twrp" path="device/zte/P809T70"  remote="github" revision="android-8.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_P809T70-eng
mka recoveryimage
```
