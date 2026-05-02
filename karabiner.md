# Karabiner

Short verification note for Karabiner-Elements key names.

## Status

Karabiner coverage in `keys.json` is complete for actual keys.

- Verified against the Karabiner-Elements source listed in `sources.md`.
- Checked both `name_value_pairs` and `other_usage_page_pairs`.
- Existing canonical keys keep their own names; Karabiner names live under the `karabiner-elements` field on those entries.

## Exception

- `vk_none` is intentionally not represented as a canonical key.
- It is a Karabiner sentinel/no-key placeholder, not a real key identity.
