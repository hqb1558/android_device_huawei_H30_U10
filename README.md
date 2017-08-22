## TWRP device tree for Huawei Honor 3C (H30_U10)

Add to `.repo/local_manifests/H30_U10.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/huawei/H30_U10" name="android_device_huawei_H30_U10" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_H30_U10-eng
make -j5 recoveryimage
```