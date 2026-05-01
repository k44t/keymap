# keymap

Cross-platform keyboard key inventory extracted from `mappy`.

## Contents

- `keys.json`: canonical key inventory covering HID, Linux, Windows, Mac, Web, and related metadata.

## Notes

- Code-like numeric fields are stored as hex strings in JSON using the `0x...` form.
- HID usages are split into `hid.page-num` and `hid.code`.
- Some platform mappings intentionally collapse onto shared native identities; those entries use `aliasOf` and include a short comment.

## License

MIT
