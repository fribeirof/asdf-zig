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
asdf plugin-add zig https://github.com/zigcc/asdf-zig.git
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

## License

Licensed under the
[Apache License, Version 2.0](https://www.apache.org/licenses/LICENSE-2.0).
