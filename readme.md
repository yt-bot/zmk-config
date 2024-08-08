# QWERTY fork of urob's zmk config

This config is work in progress. The keymap supports Linux and MacOS, and doesn't have Windows specific settings. Note that the included keymap image file does not reflect the current keymap apart from combos.

The build script supports Glove80 and 42 key Corne keyboards.

Notable changes:

- QWERTY layout
- has separate layers for English and Swedish layouts on Linux and Macos.
  - Linux: set the host keyboard layout to en-US.
  - Macos: set the host keyboard layout to unicode (U+). base.keymap has a Mac layer that uses SV variants of symbol keys, but SV_LT and SV_GT are always replaced with section and degree symbols when the host's keyboard layout is set to SE/FI. This happens at least with MacOS Sonoma. Hence, use unicode on host for SV layout (or both).
- has a separate symbol layer in addition to the original combos.
- mouse layer is removed for the time being.

TODO:

- add navigation layers for lefts hand usage.
- unify the layers in base.keymap where possible and remove unused layers.
- fix broken combos (sv/macos).
