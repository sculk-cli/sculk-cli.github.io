> This page assumes you have read '[How It Works](../how-it-works.md)'

There are two ways to start a Sculk modpack:

1. Using the [`sculk init`](../commands/init.md) command. Enter a new empty
   directory in the command line, and run the init command. You will be prompted
   for several inputs before a skeleton modpack is created.
2. Importing an existing pack from Modrinth or Curseforge (Packwiz import
   support is planned in the future): run
   [`sculk import mr <path to .mrpack>`](../commands/import/mr.md) or
   [`sculk import cf <path to curseforge pack .zip>`](../commands/import/cf.md).
   This imports all of the projects and files from the existing modpack,
   converting them to Sculk manifests where possible.

You can also look at the [example modpack](https://github.com/sculk-cli/example)
for an example of a fully functioning pack that implements all of the guides on
this site.

!!! info

    You can type to filter list prompts such as the Minecraft version prompt.

Use the [`sculk add mr <search query or mod slug>`](../commands/add/mr.md),
[`sculk add cf <search query or mod slug>`](../commands/add/cf.md), or [`<sculk add url>`](../commands/add/url.md) commands to add
mods (or shaderpacks, datapacks, etc.) to your modpack. To add files such as
configs, just place the file in the correct folder and run `sculk refresh`.

!!! info

    If you have a file which you _do not_ want to be added when you run `sculk refresh`, add it to a `.sculkignore` file.

To test your modpack, run [`sculk install <path to modpack folder>`](../commands/install.md) in a
`.minecraft` folder - you can add this as a pre-launch command if your launcher
supports it.

Once you are familiar with the basics, you can take a look at the other guides
on this site, as well as documentation for specific commands.
