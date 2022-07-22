*Modern systems programming language design experiment*
# Data Types



## Character

* internal (24-bit?)
* TBD: list of special characters
* https://www.unicode.org/Public/14.0.0/ucd/NamesList.txt
* https://www.unicode.org/Public/14.0.0/ucd/NameAliases.txt
* TBD: \x -> get from enum / constant mapping / and maybe also dynamically?

Inferred definition:

    var c = 'a';
    var c = '\n';
    var c = '\u123';
    var c = '\U+123ABC';
    var c = '\U{123ABC}';
    var c = '\U{Pile of Poo}';
    var c = '\U+200B{ZERO WIDTH SPACE}'; // will warn on mismatch

Explicit conversion:

    var c = 0x123ABC std:char;

Declaration:

    TBD

## String

* core language feature
* unspecified internal representation, SSO or COW, until raw data are requested
* TBD: raw strings implemented in editor by inserting U+02 (STX) and end by U+03 (ETX) or NUL?, with nesting support
* http://www.unicode.org/Public/UCD/latest/ucd/NamedSequences.txt
* https://www.unicode.org/Public/14.0.0/ucd/NamedSequences.txt
* https://www.unicode.org/Public/emoji/4.0/emoji-sequences.txt
* https://www.unicode.org/Public/emoji/4.0/emoji-zwj-sequences.txt
* 

## Inferred definition:

    var s = "Hello World!";
    var s = "Hello World!" #utf-16; // suggests internal storage

## Integer types

* 2-complement binary



## Floating point types IEE-754





