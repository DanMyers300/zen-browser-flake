# Zen Browser

This is a flake for the Zen browser.

Just add it to your NixOS `flake.nix` or home-manager:

```nix
inputs = {
  zen-browser.url = "github:DanMyers300/zen-browser-flake";
  ...
}
```

## Packages

Then in the `configuration.nix` in the `environment.systemPackages` add:

```nix
inputs.zen-browser.packages."${system}".default
```

```shell
$ sudo nixos-rebuild switch
$ zen
```
