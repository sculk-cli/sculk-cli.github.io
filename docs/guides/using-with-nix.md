Sculk provides a Nix flake which contains the package itself, as well as a function to fetch a Sculk modpack as a derivation.

Support is only provided for users using flakes.

# Installing Sculk

In `flake.nix`:

```nix
sculk = {
	url = "github:sculk-cli/sculk?dir=nix";
	inputs.nixpkgs.follows = "nixpkgs";
};
```

Then run `nix flake update`.

You can add Sculk as a package using `inputs.sculk.packages.<system>.sculk`.

# Using `fetchSculkModpack`

Below is an example of how to use the `fetchSculkModpack` function along with [nix-minecraft](https://github.com/Infinidoge/nix-minecraft).

```nix
services.minecraft-servers = let
  modpack = inputs.sculk.lib.fetchSculkModpack { inherit (pkgs) stdenvNoCC jre_headless; sculk = inputs.sculk.packages.x86_64-linux.sculk; } {
    url = "https://raw.githubusercontent.com/Jamalam360/pack/bd19d74601963becab9eb1232d12412133132812";
    hash = "sha256-gQl2yx2V6wuF96wmHwSdEgQUHyP2zKFbe8/EPfUgbUY=";
  };
in {
  enable = true;
  eula = true;
  openFirewall = true;
  dataDir = "/var/lib/minecraft-servers";

  servers.minecraft-server = {
    enable = true;
    package = pkgs.minecraftServers.fabric-1_20_1;
    autoStart = true;
    restart = "always";
    symlinks = {
      "mods" = "${modpack}/mods";
    };
    jvmOpts = "-Xmx10G -Xms10G";
  };
};
```
