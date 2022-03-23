[Click here to go to the live utility.](https://aaronsantiago.github.io/qmk-to-zmk/)

# QMK to ZMK

This is a utility for converting JSON files from the [QMK Configurator](https://config.qmk.fm/) into ZMK keymap files. To use, paste your JSON file into the left input, and the output keymap will be in the right text input.

An example JSON that has been tested to import properly into ZMK is [here](https://github.com/aaronsantiago/zmk-config/blob/main/lily58_rev1_layout_mine.json).

## Special Keys
For any specific ZMK commands you might need, like bluetooth keys, use the ANY key and type in the entire ZMK command including the ampersand, for example:

`&bt BT_SEL 0`

This utility is a work in progress so there are missing keys and functionalities. I'm accepting pull requests to fill in keys, correct any errors, or add more functionalities.

Any keys that I could not figure out the correct mapping I set to F20, so I invite contributors with more knowledge to help out!

## Contributing: Architecture and Design

This utility is intentionally designed as a lightweight, single file. It works both hosted and as a downloaded HTML file for offline use.

For functionality, this should generally be limited to anything from QMK that can be trivially translated into ZMK.

Some useful references:
 - [QMK Keycodes](https://github.com/qmk/qmk_firmware/blob/master/docs/keycodes.md)
 - [ZMK Keycodes](https://zmk.dev/docs/codes/)
 - [ZMK Behaviors](https://zmk.dev/docs/behaviors/layers)
