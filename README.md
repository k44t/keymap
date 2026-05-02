# keymap

Cross-platform keyboard key inventory extracted from `mappy`.

## Contents

- `keys.json`: canonical key inventory keyed directly by canonical key name.
- `autohotkey.md`: short coverage note for the AutoHotkey key vocabulary.
- `karabiner.md`: short coverage note for the Karabiner-Elements key vocabulary.
- `divergence.md`: notes on remaining semantic divergence across platforms and software vocabularies.
- `sources.md`: upstream source links used for the current mappings and audits.

## Notes

- Code-like numeric fields are stored as hex strings in JSON using the `0x...` form.
- `keys.json` is a flat top-level map of canonical key names to per-platform and per-tool metadata.
- HID usages are split into `hid.page-num` and `hid.code`.
- Some platform mappings intentionally collapse onto shared native identities; those entries use `aliasOf` and include a short comment.

## License

MIT
