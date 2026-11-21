# ProdCut releases

Installers and the `manifest.json` the app's Version page reads. Nothing is
developed here: this repository exists so a ProdCut build can look up its own
releases without reaching into the source tree.

Each release carries, per platform and architecture:

- `ProdCut-<version>-<platform>-<arch>-setup.exe` and `.msi` (Windows)
- `ProdCut-<version>-macos-<arch>.dmg` (macOS)
- `.deb`, `.rpm`, `.AppImage` and `.pkg.tar.zst` (Linux)
- `manifest.json`: every file's URL, size and SHA-256, checked before install
- `ProdCut-<version>-source.tar.gz`: the corresponding source of that build

ProdCut is a fork of [Concat](https://github.com/jub0t/Concat) and the code in
each release is licensed **AGPL-3.0-or-later**, which is why the source travels
with the binaries above. Report bugs wherever you were given the product.
