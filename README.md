# Local Manifests

These are local manifests for various devices.


# Usage:
You can place the text in the .repo/local_manifests/manifest.xml after `repo init $SOME_ROM_MANIFEST_URL` by either:

manually creating .repo/local_manifests and a .xml file and then copying the code to .repo/local_manifests/manifest.xml.

OR

running
```
mkdir .repo/local_manifests
```
```
curl https://raw.githubusercontent.com/AodX/local_manifests/main/$DEVICE/$MANIFEST_NAME > .repo/local_manifests/manifest.xml
```
be sure to replace $DEVICE and $MANIFEST_NAME with a device codename and manifest name, that are available.

Example:
```
mkdir .repo/local_manifests && curl https://raw.githubusercontent.com/Zed9K/local_manifests/main/A14Lineage.xml > .repo/local_manifests/manifest.xml
```

after that do 
```repo sync --force-sync --no-tags --no-clone-bundle -c```
to get both the rom and device sources.
