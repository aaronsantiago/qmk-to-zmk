*[Click here to go to the live utility.](https://aaronsantiago.github.io/qmk-to-zmk/)

#QMK to ZMK

This is a utility for converting JSON files from the QMK Configurator into ZMK keymap files. To use, paste your JSON file into the left input, and the output keymap will be in the right text input.

##Special Keys
For any specific ZMK commands you might need, like bluetooth keys, use the ANY key and type in the entire ZMK command including the ampersand, for example:

`&bt BT_SEL 0`

Most behaviors such as Mod-Taps, Layer-Taps, etc. are supported, except for any that don't exist in ZMK like Tap Dance.

*HOWEVER*, this utility is a work in progress so there may be some missing keys or functionalities. I'm accepting pull requests to fill in keys, correct any errors, or add more functionalities.

Any keys that I could not figure out the correct mapping I set to F20, so I invite contributors with more knowledge to help out!

##Architecture and Design

This utility is intentionally designed as a lightweight, single file. It works both hosted and as a downloaded HTML file for offline use.

For functionality, this should generally be limited to anything from QMK that can be trivially translated into ZMK.