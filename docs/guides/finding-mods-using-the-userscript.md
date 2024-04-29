Sculk provides a [Tampermonkey](https://www.tampermonkey.net/) userscript which
can be used to add mods to a Sculk modpack from Modrinth and Curseforge. It can
be found [here](https://github.com/sculk-cli/sculk/blob/main/userscript.js).

Once it is installed, there are 3 buttons added to every project page on
Modrinth and Curseforge:

1. "Add to Sculk Install List": adds a project to the install list
2. "Export Sculk Install List": exports the install list to a file
3. "Clear Sculk Install List": clears the install list

Once the list is exported, you can use the
[`sculk add list <path to list file>`](../commands/add/list.md) to install all
the mods in the list.
