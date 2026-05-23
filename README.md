# Corne Typeractive 5x3 ZMK Config

![Current keymap](docs/corne.svg)

## Quick Read

This is a compact daily-driver Corne setup for a Typeractive 5x3 build. The base layer keeps letters on the main grid, puts `lower` and `raise` on the thumbs, and uses home-row mods for the core modifiers.

The firmware now uses `five_column_transform`, so each layer has exactly 36 positions: 3 rows of 10 keys plus 6 thumb keys. This matches the physical 5-column keyboard and avoids carrying the virtual outer columns from a 6-column Corne layout.

The build matrix targets `nice_nano//zmk`, which keeps the GitHub Actions firmware build aligned with the current ZMK board naming and the nice!view adapter setup.

## Layout Notes

- Base: QWERTY with bilateral home-row mods. Left-hand mods only trigger with right-hand keys, and right-hand mods only trigger with left-hand keys.
- Combos: `Q` + `W` sends `Esc`; `O` + `P` sends `Backspace`.
- Lower: numbers, Bluetooth profile keys, arrows, and media controls.
- Raise: common symbols, brackets, slash/backslash, quotes, backtick, and tilde.
- Thumbs: `Tab`, `Lower`, `Space`, `Enter`, `Raise`, and `Backspace`.

Things still worth adding for daily work:

- Complete the navigation layer with `HOME`, `END`, `PG_UP`, `PG_DN`, `DEL`, and maybe `INS`.
- Add `F1` through `F12`, especially for IDEs, terminals, browser devtools, and debugging.
- Complete the Bluetooth profile keys with `BT_SEL 0` and `BT_SEL 1`, in addition to profiles 2, 3, and 4.
- Consider adding a small system layer for reset, bootloader, output switching, and screenshot/lock shortcuts.

## Keymap Drawing

The image above is generated with [`keymap-drawer`](https://github.com/caksoylar/keymap-drawer). The `Draw keymap` workflow parses `config/corne.keymap`, writes the generated YAML to `docs/corne.yaml`, and renders `docs/corne.svg` for the README.
