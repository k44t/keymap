# AutoHotkey

Short verification note for AutoHotkey key names.

## Status

AutoHotkey coverage in `keys.json` is complete for keyboard keys and named mouse buttons that belong in this inventory.

- Verified against the AutoHotkey v2 key list.
- Source link is listed in `sources.md`.
- Named keys are represented either directly or as aliases under the `autohotkey` field on canonical entries.
- `Media_Stop` is represented under canonical `media-stop`.
- Mouse buttons are represented under canonical mouse-button entries such as `mouse-left` and `mouse-side`.

## Intentional Non-Keys

- Generic modifier words such as `Control`, `Ctrl`, `Alt`, and `Shift` are not separate canonical keys here.
- `CtrlBreak` is treated as behavior on `pause`, not as its own physical key.
- Wheel events such as `WheelUp` and `WheelDown` are intentionally out of scope here because they are pointer-wheel events, not key identities.
