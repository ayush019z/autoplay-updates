# AutoPlay Updates

Public update metadata and downloadable Android releases for Cricket Auto Assist / AutoBowl.

- Update manifest: [version.json](./version.json)
- The Android app checks this manifest to see whether a newer version is available.
- APK releases are published as GitHub Release assets named `Autobowl.apk`.

## Publishing a new Android version

1. Build a release APK from the private `ayush019z/Autobowl-` source repository.
2. Increase `versionCode` and update `versionName` in `version.json`.
3. Create a release in this repository and upload the APK with the exact asset name `Autobowl.apk`.
4. Update `releaseNotes` and commit `version.json`.

**Important:** Android only installs an update over an existing install if the APK is signed with the same signing key. Keep the release signing key backed up securely. Do not upload signing keys or passwords to this public repository.
