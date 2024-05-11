Finds Curseforge/Modrinth projects for files in the manifest.

## Usage

- `sculk link <target>`
- `sculk link -y <target>`

## Options

- `<target>` (one of `modrinth`, `curseforge`): the site to find projects from.
- `<y>, <yes>`: automatically accept matches without prompting.

## Example

- Run `sculk add modrinth fabric-api`
- Run `sculk link curseforge`
- You now have a Fabric API manifest with both a Modrinth and Curseforge source.
