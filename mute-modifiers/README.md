# Ignore Modifiers

Selectively suppresses handling of modifiers when specific windows are active. Windows are identified by URL. This allows modifiers like <kbd>Search</kbd> and <kbd>Assistant</kbd> to pass through as normal keyboard events to the active application, which is useful for remote control applications (e.g. Citrix Receiver & Workspace).

Non-keyboard events (e.g. touchpad gestures, mouse, etc.) are unaffected.

# Related Work

* Chrome [input.ime](https://developer.chrome.com/docs/extensions/reference/input_ime/) Extension API
* Chrome [windows.getCurrent](https://developer.chrome.com/docs/extensions/reference/windows/#method-getCurrent) Extension API
* [chromeos-key-remapper](https://github.com/ento/chromeos-key-remapper/blob/master/remapper/engine.js) translates keys, excluding when `crosh` is active
