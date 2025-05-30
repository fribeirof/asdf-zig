# asdf-zig

[Zig](https://ziglang.org) plugin for asdf version manager

## Installation
* First install [asdf](https://asdf-vm.com/guide/getting-started.html)
* Then install asdf-zig

```bash
asdf plugin add zig https://github.com/fribeirof/asdf-zig.git
# Update to latest if already installed
asdf plugin update zig
```

* Then either install latest (tagged) Zig version
```bash
asdf install zig latest
asdf set -u zig latest
zig version
```

* Or a specific version/build (dev or tagged)
```bash
# dev build
asdf install zig 0.15.0-dev.666+c04be630d
asdf set -u zig 0.15.0-dev.666+c04be630d
zig version

# or tagged
asdf install zig 0.14.1
asdf set -u zig 0.14.1
zig version
```

## Usage

Check [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to
install & manage versions.

### Zig download mirror

As suggested in [Migrating from AWS to Self-Hosting
](https://ziglang.org/news/migrate-to-self-hosting/), asdf-zig will first try download from mirrors.

The mirrors list is synced with [setup-zig](https://github.com/mlugg/setup-zig/blob/main/mirrors.json) from time to time.

You can also configure where to download `index.json` with `ASDF_ZIG_INDEX_URL` env var, it's https://ziglang.org/download/index.json by default.

## License

Licensed under the
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
