The Sculk manifest is versioned such that new features can be added without
breaking existing modpacks. The `formatVersion` key in the root manifest defines
the current format version for the modpack.

Modpacks using an old format version will not work and have to be migrated using
the [`sculk migrate`](../commands/migrate.md) command. Some migrations may take
some time, as they may have to make web requests or download files.

The current latest version is **1.1**.

## Changelog

### V1.0

- Initial public alpha release.

### V1.1

- Add a `murmur2` field to the `hashes` object of file manifests.
