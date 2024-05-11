Initialize a new Sculk modpack.

## Usage

- `sculk init` (input options via prompts and have path default to `.`)
- `sculk init <path>` (input options via prompts)
- `sculk init --name <name> --loader <loader> --minecraft-version <minecraft_version> <path>`

## Options

- `<path>`: the path to the modpack folder.
- `<name>`: the name of the modpack.
- `<loader>` (one of `forge`, `fabric`, `neoforge`, `quilt`): the mod loader to
  use.
- `<minecraft_version>`: the Minecraft version to use.
