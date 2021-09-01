*Modern systems programming language design experiment*
# Data Types



## Character

* internal (24-bit?)

Inferred definition:

    var c = 'a';
    var c = '\n'
    var c = '\u+123ABC'

Explicit conversion:

    var c = 0x123ABC std:char;

Declaration:

    TBD

String

* core language feature
* unspecified internal representation, SSO or COW, until raw data are requested
* 

Inferred definition:

    var s = "Hello World!";
    var s = "Hello World!" #utf-16; // suggests internal storage

Integer types

* 2-complement binary



Floating point types IEE-754





