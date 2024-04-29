# Fields

## `name`

- description: The name of the modpack. Used in exports.
- type: `string`

## `version`

- description: The version of the modpack. Used in exports.
- type: `string` (semver, ideally)

## `loader`

- description: The mod loader to use and its version.
- type: `object`

### `loader.type`

- description: The mod loader to use
- type: `fabric | forge | neoforge | quilt`

### `loader.version`

- description: The version to use for the mod loader
- type: `string`

## `manifests`

- description: The manifests included in the pack.
- type: `array`

### `manifests[].path`

- description: The path to the manifest.
- type: `string` (path, ends with `.sculk.json` and is relative to the root manifest) 

### `manifests[].sha256`

- description: The SHA256 hash of the manifest file.
- type: `string` 

## `files`

- description: The files included in the pack.
- type: `array`

### `files[].path`

- description: The path to the file.
- type: `string` (path) 

### `files[].sha256`

- description: The SHA256 hash of the file.
- type: `string` 

### `files[].side`

- description: The side that the file should be installed on.
- type: `client_only | server_only | both`
