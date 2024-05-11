The Sculk manifest is versioned such that new features can be added without
breaking existing modpacks. The `formatVersion` key in the root manifest defines
the current format version for the modpack.

Old modpacks will be automatically migrated to the latest version when any Sculk
command is run.

The current latest version is **1.0**.

## Changelog

### V1.0

- Initial public alpha release.

### V1.1

- Add a `murmur2` field to the `hashes` object of file manifests.
