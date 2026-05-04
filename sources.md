# sources

This file preserves the source taxonomy previously embedded in `keys.json`.

`keys.json` is now just the canonical key map itself, so the shared source metadata lives here instead.

## hid

- define: <https://www.usb.org/sites/default/files/hut1_5.pdf>
- map: none

## linux-evdev

- define: <https://raw.githubusercontent.com/torvalds/linux/master/include/uapi/linux/input-event-codes.h>
- map: <https://raw.githubusercontent.com/torvalds/linux/master/drivers/hid/hid-input.c>

## linux-xkb-keycode

- define: <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/dom/dom_code_data.inc>
- map:
  - <https://raw.githubusercontent.com/torvalds/linux/master/drivers/hid/hid-input.c>
  - <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/dom/dom_code_data.inc>

## linux-xkb-keysym

- define: <https://raw.githubusercontent.com/xkbcommon/libxkbcommon/master/include/xkbcommon/xkbcommon-keysyms.h>
- map:
  - <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/dom/dom_code_data.inc>
  - <https://raw.githubusercontent.com/xkbcommon/libxkbcommon/master/include/xkbcommon/xkbcommon-keysyms.h>

## windows-scancode

### scancode

- define: <https://learn.microsoft.com/en-us/windows/win32/inputdev/about-keyboard-input>
- map: <https://learn.microsoft.com/en-us/windows/win32/inputdev/about-keyboard-input>

### appcommand

- define: <https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-appcommand>
- map: <https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-appcommand>

## windows-virtual

### default

- define: <https://learn.microsoft.com/en-us/windows/win32/inputdev/virtual-key-codes>
- map: <https://learn.microsoft.com/en-us/windows/win32/inputdev/about-keyboard-input>

### appcommand

- define: <https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-appcommand>
- map: <https://learn.microsoft.com/en-us/windows/win32/inputdev/wm-appcommand>

## mac

### virtual-keycode

- define: <https://raw.githubusercontent.com/phracker/MacOSX-SDKs/master/MacOSX10.15.sdk/System/Library/Frameworks/Carbon.framework/Versions/A/Frameworks/HIToolbox.framework/Versions/A/Headers/Events.h>
- map: <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/keyboard_code_conversion_mac.mm>

### function-character

- define: <https://raw.githubusercontent.com/phracker/MacOSX-SDKs/master/MacOSX10.15.sdk/System/Library/Frameworks/AppKit.framework/Versions/C/Headers/NSEvent.h>
- map:
  - <https://raw.githubusercontent.com/phracker/MacOSX-SDKs/master/MacOSX10.15.sdk/System/Library/Frameworks/AppKit.framework/Versions/C/Headers/NSEvent.h>
  - <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/keyboard_code_conversion_mac.mm>

### media-event

- define: <https://raw.githubusercontent.com/apple-oss-distributions/IOHIDFamily/main/IOHIDSystem/IOKit/hidsystem/ev_keymap.h>
- map:
  - <https://raw.githubusercontent.com/apple-oss-distributions/IOHIDFamily/main/IOHIDSystem/IOKit/hidsystem/ev_keymap.h>
  - <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/dom/dom_code_data.inc>

### system-defined-subtype

- define: <https://raw.githubusercontent.com/apple-oss-distributions/IOHIDFamily/main/IOHIDSystem/IOKit/hidsystem/IOLLEvent.h>
- map: <https://raw.githubusercontent.com/apple-oss-distributions/IOHIDFamily/main/IOHIDSystem/IOKit/hidsystem/IOLLEvent.h>

### default

- define: <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/keyboard_code_conversion_mac.mm>
- map: <https://raw.githubusercontent.com/chromium/chromium/main/ui/events/keycodes/keyboard_code_conversion_mac.mm>

## web

- define:
  - <https://www.w3.org/TR/uievents-code/>
  - <https://www.w3.org/TR/uievents-key/>
- map:
  - <https://www.w3.org/TR/uievents-code/>
  - <https://www.w3.org/TR/uievents-key/>

## qmk

- define: <https://docs.qmk.fm/keycodes>
- map: <https://docs.qmk.fm/keycodes>

## kmonad

- define: <https://kmonad.org/>
- map: <https://kmonad.org/>

## kanata

- define: <https://github.com/jtroo/kanata>
- map: <https://github.com/jtroo/kanata>

## keyd

- define: <https://raw.githubusercontent.com/rvaiya/keyd/refs/heads/master/docs/keyd.scdoc>
- map: <https://raw.githubusercontent.com/rvaiya/keyd/refs/heads/master/docs/keyd.scdoc>

## karabiner-elements

- define: <https://karabiner-elements.pqrs.org/docs/json/complex-modifications-manipulator-definition/key-code/>
- map: <https://karabiner-elements.pqrs.org/docs/json/complex-modifications-manipulator-definition/key-code/>

## autohotkey

- define: <https://www.autohotkey.com/docs/v2/KeyList.htm>
- map: <https://www.autohotkey.com/docs/v2/KeyList.htm>
