Adds a project to the manifest from a direct download URL.

## Usage

- `sculk add url` (input options via prompts)
- `sculk add url --slug <slug> --url <url> --filename <filename> --type <type> --side <side>`

## Options

- `slug`: the slug of the project, used for naming the file manifest.
- `url`: the download URL of the file.
- `filename`: the file name.
- `type` (one of `mod`, `shaderpack`, `resourcepack`, `datapack`): the type of
  the project.
- `side` (one of `both`, `client_only`, `server_only`): the side the project is
  for.
