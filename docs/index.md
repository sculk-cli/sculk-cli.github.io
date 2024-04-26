![Sculk: a program for creating Minecraft modpacks](https://github.com/sculk-cli/sculk/blob/main/banner.png?raw=true)


> **Warning**
> Sculk is still in early development and may be unstable

Sculk is a CLI tool for creating Minecraft modpacks, much like Packwiz. It is **aimed at modpack creators**, rather than users (for users, a program such as [Ferium](https://github.com/gorilla-devs/ferium) is recommended)

## Why Sculk?

- **Multi-source support**: Sculk allows one mod to have multiple sources (e.g. Curseforge, Modrinth, and a URL). This means that you can export Modrinth and Curseforge modpacks from the same Sculk modpack.
- **Content support**: Sculk supports mods, datapacks, resource packs, and shader packs - as well as any other files you want to include in your modpack (e.g. config).
- **Ease of use**: Sculk is designed to be easy to use, with a simple command-line interface (with nice prompts!).
- **Import support**: Sculk allows you to convert an existing Modrinth, Curseforge, or Packwiz modpack into a Sculk modpack.
- **Dependency management**: Sculk automatically installs dependencies for you, and will keep track of them so that they can be removed if their dependant is.
- _[Planned]_ **Rollback system**: Sculk keeps track of changes made to the modpack, so that you can easily revert changes - because it's too easy to forget to keep your Git commits granular.
- _[Planned]_ **Publishing support**: Sculk can export to Curseforge and Modrinth modpacks, and can even publish them for you from the command line.

## How?

_TODO: packaging solution and docs on it here_

Once Sculk is installed and on your `PATH`, you can follow the [getting started guide](./guides/getting-started.md). 

There is also documentation on specific commands and the manifest format Sculk uses, which can be found in the navbar.
