![Sculk: a program for creating Minecraft modpacks](https://github.com/sculk-cli/sculk/blob/main/banner.png?raw=true)

!!! warning

    Sculk is still in early development and may be unstable

Sculk is a CLI tool for creating Minecraft modpacks, much like Packwiz. It is
**aimed at modpack creators**, rather than users (for users, a program such as
[Ferium](https://github.com/gorilla-devs/ferium) is recommended)

## Why Sculk?

- **Multi-source support**: Sculk allows one mod to have multiple sources (e.g.
  Curseforge, Modrinth, and a URL). This means that you can export Modrinth and
  Curseforge modpacks from the same Sculk modpack.
- **Content support**: Sculk supports mods, datapacks, resource packs, and
  shader packs - as well as any other files you want to include in your modpack
  (e.g. config).
- **Ease of use**: Sculk is designed to be easy to use, with a simple
  command-line interface (with nice prompts!).
- **Import support**: Sculk allows you to convert an existing Modrinth,
  Curseforge, or Packwiz modpack into a Sculk modpack.
- **Dependency management**: Sculk automatically installs dependencies for you,
  and will keep track of them so that they can be removed if their dependant is.
- _[Planned]_ **Rollback system**: Sculk keeps track of changes made to the
  modpack, so that you can easily revert changes - because it's too easy to
  forget to keep your Git commits granular.
- _[Planned]_ **Publishing support**: Sculk can export to Curseforge and
  Modrinth modpacks, and can even publish them for you from the command line.

## How?

To install Sculk, first make sure you have Java 17 or greater installed, then:

- On Linux/MacOS, run
  `python3 <(wget https://raw.githubusercontent.com/sculk-cli/sculk/main/install.py -q -O-)`
- On Windows, run
  `Invoke-WebRequest -Uri "https://raw.githubusercontent.com/sculk-cli/sculk/main/install.py" -OutFile "install.py"; python3 .\install.py`

!!! tip

    If you'd rather install Sculk manually, download `sculk.zip` from the [latest release](https://github.com/sculk-cli/sculk/releases/latest). Extract it and make sure that the `bin` directory is in your `PATH`

Once Sculk is installed and on your `PATH`, you can follow the
[getting started guide](./guides/getting-started.md). The
'[How It Works](./how-it-works.md)' page is also recommended before you begin.

There is also documentation on specific commands and the manifest format Sculk
uses, which can be found in the navbar.
