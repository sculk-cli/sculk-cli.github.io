Export a MultiMC-compatible (i.e. MultiMC, Prism, etc.) modpack (`.zip`).

## Usage

- `sculk export multimc`
- `sculk export multimc --pack-url <pack_url>
- `sculk export multimc --pack-url <pack_url> --sculk-jar-location <sculk_jar_location>

## Options

- `pack_url`: the URL (or local path) to download/update the pack from (see the [installing from GitHub](../../guides/installing-from-github.md) if you are using GitHub).
- `sculk_jar_location`: the path of `sculk.jar`, to use for auto updating. If unspecified, Sculk will try to automatically resolve its location.
