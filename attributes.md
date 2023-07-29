*Modern systems programming language design experiment*
# Attributes

Attributes serve various functions. They are used to annotate, optimize code generation or improve diagnostics.
In general, the compiler is allowed to ignore most of the attributes.
They are generally permitted to observably affect the execution, although the code must not rely on such side effects.

## Syntax

    #name
    #name:parameter
    #name:parameter,parameter
    #name:parameter=value,parameter=value

* there is no space between `#` character and attribute name
* attribute is terminated by first white-space or a character not part of attribute's parameter token
* *name* and *parameter* follow rules for [identitiers](identifiers.md)

## Semantics

* after a thing they affect, even after semicolon
* typically at the end of the row, after the the whole statement the affect
* user-defined?

## [Source code file character set](charset.md)

    #UTF-8

## Epochs

* epoch is a version of the language that is syntactically or semantically backwards incompatible
* on a global scope specifies the epoch until the end of the file, or different `#language` attribute
* can be applied to any local scope

    #language:1
    #language:standard
    #language:1.4-preview

Case-insensitive, changes how the source code file data are interpreted immediately following the terminating semicolon.

## TBD

    #uninitialized // keep stack trash
    #deferred // evaluation may/should be deferred to any point before first use
    #idempotent // repeated evaluation gives the same result (may read global state)
    #unsequenced // https://www.open-std.org/jtc1/sc22/wg14/www/docs/n2956.htm
    #reproducible
    #ignore-exceptions // any thrown exception is caught and ignored

...

