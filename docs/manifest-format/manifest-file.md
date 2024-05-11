A manifest file is any file that ends with `.sculk.json` and is not the root manifest.

# Fields

## `filename`

- description: The name of the downloaded file.
- type: `string`

## `side`

- description: The side that the file should be installed on.
- type: `client_only | server_only | both`

## `hashes`

- description: The hashes of the downloaded file.
- type: `object`

### `hashes.sha1`

- description: The SHA1 hash of the downloaded file.
- type: `string`

### `hashes.sha512`

- description: The SHA512 hash of the downloaded file.
- type: `string`

### `hashes.murmur2`

- description: The Murmur2 (Curseforge variant) hash of the downloaded file.
- type: `int`

## `fileSize`

- description: The size of the downloaded file, in bytes.
- type: `int`

## `sources`

- description: The sources that can be used to download the file.
- type: `object`

### `sources.curseforge`

- description: The Curseforge source.
- type: `object?`

#### `sources.curseforge.projectId`

- description: The Curseforge project ID.
- type: `int`

#### `sources.curseforge.fileId`

- description: The Curseforge file ID.
- type: `int`

#### `sources.curseforge.fileUrl`

- description: The Curseforge file download URL.
- type: `string`

### `sources.modrinth`

- description: The Modrinth source.
- type: `object?`

#### `sources.modrinth.projectId`

- description: The Modrinth project ID.
- type: `string`

#### `sources.modrinth.fileUrl`

- description: The Modrinth file download URL.
- type: `string`
 
### `sources.url`

- description: The URL source.
- type: `object?`

#### `sources.modrinth.url`

- description: The file download URL.
- type: `string`
 
