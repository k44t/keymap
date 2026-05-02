# divergence

Remaining semantic divergence notes across platforms and software vocabularies.

## Current issues

### menu vs compose

- Canonical `menu` and canonical `compose` are distinct in this inventory.
- `keyd`, Karabiner-Elements, AutoHotkey, and the platform-native fields keep that distinction.
- Kanata currently does not: its `ContextMenu` / `menu` / `apps` / `comp` / `cmps` / `cmp` name family resolves to `KEY_COMPOSE` in the upstream source listed in `sources.md`.
- Current modeling reflects Kanata's actual behavior by attaching that family to canonical `compose` and leaving canonical `menu` without a Kanata mapping.

### email vs mail

- Linux distinguishes `KEY_EMAIL` from `KEY_MAIL`.
- Other stacks tend to flatten launcher semantics toward the generic mail-launch concept.
- Canonical `email` is therefore Linux-shaped and narrower than canonical `mail`.
- This is reflected in `keys.json` comments and in the current tool mappings.

### ISO/locale key collapse

- `iso-intl-backslash` is broadly distinguishable across stacks, but under different names: `nubs`, `102nd`, `IntlBackslash`, `non_us_backslash`, `SC056`.
- `iso-#` is not broadly distinguishable: Linux and several higher-level stacks collapse it onto backslash-like behavior, while Karabiner-Elements still exposes `non_us_pound`.
- This means the two ISO-only keys are not treated symmetrically across ecosystems.

### yen/backslash locale behavior

- Kanata accepts parser alias `yen` for the backslash key, but also accepts the actual Unicode `¥` for canonical `intl-yen`.
- That reflects locale compatibility behavior rather than a stable cross-platform identity.
- `keys.json` currently models both facts explicitly.

### JIS / IME key family

- The Japanese/IME-related keys remain the biggest unresolved cross-platform divergence cluster.
- Important entries include `kana`, `katakana`, `hiragana`, `henkan`, `muhenkan`, and the `eisu`/`Lang2` family.
- Web, Linux, Windows scancode-level naming, Karabiner-Elements, and Kanata do not line up on one shared vocabulary here.
- Kanata is especially likely to need platform-specific modeling for these keys because its upstream source maps some of them differently by target platform.

## Resolved / not treated as semantic issues

- `print` / `sysrq` / `PrintScreen`: treated as naming divergence on the same key, not a semantic split.
- Kanata `break` / `brk`: treated as aliases of canonical `pause`, matching upstream Kanata mapping to `KEY_PAUSE`.
