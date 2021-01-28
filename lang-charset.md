*Modern systems programming language design experiment*
# Source code file format and basic character set

The only encoding the implementation is required to support is [UTF-8](https://en.wikipedia.org/wiki/UTF-8).

Change in character set must be preceeded either by BOM or by an [lang-attr.md](attribute) on a separate line, e.g.:

    #utf-8

## Basic character set

Outside of character/string literals and comments, the basic character set matches that of C++ (see [C++ Phases of translation](https://en.cppreference.com/w/cpp/language/translation_phases)) plus several additional characters found under [AltGr](https://en.wikipedia.org/wiki/AltGr_key) on [US International keyboard layout](https://en.wikipedia.org/wiki/QWERTY#US-International).

Only characters that can be typed directly (not using other program/flyout or Alt+# combination) are to be used.

Code | Character | Keypress | Used
-|-|-|-
U+00A1 | ¡ | AltGr + 1
U+00B9 | ¹ | AltGr + 1 + Shift
U+00B2 | ² | AltGr + 2
U+00B3 | ³ | AltGr + 3
U+00A4 | ¤ | AltGr + 4 | Yes
U+00D7 | × | AltGr + = | Yes
U+00F7 | ÷ | AltGr + = + Shift | Yes
-|-|-|-
U+00AE | ® | AltGr + R
U+00AB | « | AltGr + [
U+00BB | » | AltGr + ]
U+00AC | ¬ | AltGr + \
U+00A6 | ¦ | AltGr + \ + Shift
-|-|-|-
U+00F8 | ø | AltGr + L
U+00D8 | Ø | AltGr + L + Shift
U+00B6 | ¶ | AltGr + ;
U+00B0 | ° | AltGr + ; + Shift
U+00B4 | ´ | AltGr + '
U+00A8 | ¨ | AltGr + ' + Shift
-|-|-|-
U+00A9 | © | AltGr + C
U+00B5 | µ | AltGr + M

# Experimental ideas

...

