# Local Manifests

These are local manifests for dumpling and cheeseburger ( Oneplus 5 and 5T ).


# Usage:
You can place the text in the .repo/local_manifests/roomservice.xml after `repo init $SOME_ROM_MANIFEST_URL` by either:

manually creating .repo/local_manifests and a .xml file and then copying the code to .repo/local_manifests/roomservice.xml.

OR

running
```
mkdir .repo/local_manifests
```
```
curl https://raw.githubusercontent.com/Zed9K/local_manifests/main/$DEVICE/$MANIFEST_NAME > .repo/local_manifests/roomservice.xml
```
be sure to replace $DEVICE and $MANIFEST_NAME with a device codename and manifest name, that are available.

Example:
```
mkdir .repo/local_manifests && curl https://raw.githubusercontent.com/Zed9K/local_manifests/main/Rising-A15.xml > .repo/local_manifests/roomservice.xml
```

after that do 
```repo sync --force-sync --no-tags --no-clone-bundle -c```
to get both the rom and device sources.
