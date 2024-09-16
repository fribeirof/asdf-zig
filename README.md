# asdf-zig

[Zig](https://ziglang.org) plugin for asdf version manager

## Installation
First install [asdf](https://asdf-vm.com/guide/getting-started.html)
```bash
git clone https://github.com/asdf-vm/asdf.git ~/.asdf --branch v0.14.0
cat <<'EOF' >> $HOME/.bashrc
source "$HOME/.asdf/asdf.sh"
source "$HOME/.asdf/completions/asdf.bash"
EOF
```

Then install asdf-zig

```bash
asdf plugin add zig https://github.com/zigcc/asdf-zig.git

# Update to latest if already installed
asdf plugin update zig
```

Then install latest Zig
```bash
asdf install zig latest
asdf global zig latest
zig version
```

## Usage

Check [asdf](https://github.com/asdf-vm/asdf) readme for instructions on how to
install & manage versions.

### Zig download mirror

As suggested in [Migrating from AWS to Self-Hosting
](https://ziglang.org/news/migrate-to-self-hosting/), asdf-zig will first try download from mirrors.

Currently there are(same with [setup-zig](https://github.com/mlugg/setup-zig/blob/main/mirrors.json)):
- https://pkg.machengine.org/zig
- https://zigmirror.hryx.net/zig
- https://zig.linus.dev/zig
- https://fs.liujiacai.net/zigbuilds


You can also configure where to download `index.json` with `ASDF_ZIG_INDEX_URL` env var, it's https://ziglang.org/download/index.json by default. Availables:

- https://liujiacai.net/zigbuilds/index.json

## License

Licensed under the
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
