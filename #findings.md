Saved: 2026-05-04

Keymap policy notes:

1. `keys.json` should record stable native vocabularies for explicit key or button identities.

2. For macOS gamepads, Apple GameController button names belong in `keys.json` when Apple exposes direct button properties such as:
- `ButtonA`
- `ButtonB`
- `ButtonX`
- `ButtonY`
- `ButtonMenu`
- `ButtonOptions`
- `ButtonHome`
- `LeftShoulder`
- `RightShoulder`
- `LeftTrigger`
- `RightTrigger`
- `LeftThumbstickButton`
- `RightThumbstickButton`

3. For macOS directional elements, `keys.json` should not invent fake per-direction native key identities.

4. In particular, these Apple GameController elements need extra runtime handling instead of direct `keys.json` key mappings:
- `DPad`
- `LeftThumbstick`
- `RightThumbstick`

5. The reason is that these are directional or analog elements, not four separately named native key/button properties.

6. Canonical mappings such as `gamepad-dpad-up` or `gamepad-left-thumbstick-left` may still be produced by code, but that normalization should happen in a function that interprets directional/axis state rather than by pretending the mac source vocabulary contains discrete per-direction keys.
