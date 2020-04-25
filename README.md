## TWRP device tree for Galaxy S6 edge 404SC

Add to `.repo/local_manifests/local_manifest.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/samsung/404SC" name="android_device_samsung_404SC" remote="Github" revision="android-9.0" />
	<project path="kernel/samsung/404SC" name="frankbrazillian/android_kernel_samsung_404SC" remote="github" revision="master"/>
    <project path="external/busybox" name="TeamWin/android_external_busybox" remote="github" revision="android-9.0"/>
</manifest>
```

Then run `repo sync` to check it out.

To build:


source build/envsetup.sh
lunch omni_404SC-eng
make recoveryimage
```

