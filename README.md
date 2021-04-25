# Neo 2 for ErgoDox on QWERTZ

QMK keymap for [Neo 2](https://www.neo-layout.org/).

Based on [yeldiRium/qmk-neo2](https://github.com/yeldiRium/qmk-neo2),
which is based on [mjonuschat/ergodox_osx_neo2](https://github.com/mjonuschat/ergodox_osx_neo2).


# Description

The Neo layout is an optimized German keyboard layout developed by the
Neo Users Group, supporting many Latin-based alphabets. The positions
of the letters are not only optimized for German letter frequency,
but also for typical groups of two or three letters.  English is
considered a primary target as well.

The design tries to enforce the alternating usage of both hands to
increase typing speed  and incorporates ideas from de-ergo and other
ergonomic layouts. High frequency keys are placed in the home row.
The current layout Neo 2.0 has unique features making it suited for
many target groups such as programmers, mathematicians, scientists or
LaTeX authors.

Neo is grouped into six layers, each dedicated to a special purpose.


# Layers

At the core this is a Neo 2.0 layout adjusted for the Ergodox Infinity.
The keymap is laid out expecting GNU/Linux using the German QWERTZ layout
with accent circumflex, grave, and acute all dead. That's what you get
after running `setxkbmap de`. Use `setxkbmap -option nbsp:level2 de` to
get a non-breaking space with `Shift+Space`.

Here is an overview of the implemented layers.
The file `keymap.c` contains ASCII art comments for the exact mapping.

* Layer 1: Neo layers 1 and 2: Lowercase, upppercase and typographical characters
* Layer 2: Neo layer 3: Special characters for programming
* Layer 3: Neo layer 4: WASD-like movement keys and number block
* Layer 4: unused
* Layer 5: unused
* Layer 6: Rough estimation of Ergodox Infinity DE QWERTZ layout
* Layer 7: Function keys

# Usage

* Setup the environment according to the [QMK tutorial](https://docs.qmk.fm/#/newbs_getting_started).
* Add this repository as a submodule: `git submodule add https://github.com/blipp/qmk-neo2 keyboards/ergodox_infinity/keymaps/neo2`
* Follow these instructions to build and flash: https://github.com/blipp/qmk_firmware/tree/master/keyboards/ergodox_infinity

# Useful Links and Documentation

* [QMK keycodes](https://docs.qmk.fm/#/keycodes?id=keycodes-overview)
* [How to display the current keymap table in X](https://wiki.archlinux.org/index.php/Xmodmap#Keymap_table):
  `xmodmap -pke`
* [How to list layouts, variants, and options](https://unix.stackexchange.com/a/298947) with
  `localectl`
* [List of all setxkbmap configuration options](https://unix.stackexchange.com/a/298947)
