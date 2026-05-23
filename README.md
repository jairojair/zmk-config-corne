# Corne Typeractive 5x3 ZMK Config

![Current keymap](docs/corne.svg)

## Quick Read

This is a minimal Corne setup: the base layer is mostly dedicated to letters, the thumbs hold `lower` and `raise`, and the main modifiers live on the home row.

The keymap uses `five_column_transform`, so each layer has exactly 36 positions: 3 rows of 10 keys plus 6 thumb keys. This avoids carrying the virtual outer columns from a 6-column Corne layout.

Things still worth adding for daily work:

- Complete the navigation layer with `HOME`, `END`, `PG_UP`, `PG_DN`, `DEL`, and maybe `INS`.
- Add `F1` through `F12`, especially for IDEs, terminals, browser devtools, and debugging.
- Add quotes, backtick, and tilde to `raise`; there is still enough transparent space for those symbols.
- Complete the Bluetooth profile keys with `BT_SEL 0` and `BT_SEL 1`, in addition to profiles 2, 3, and 4.

## Keymap Drawing

The image above is generated with [`keymap-drawer`](https://github.com/caksoylar/keymap-drawer). The `Draw keymap` workflow parses `config/corne.keymap`, writes the generated YAML to `docs/corne.yaml`, and renders `docs/corne.svg` for the README.
