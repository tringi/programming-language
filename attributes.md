*Modern systems programming language design experiment*
# Attributes

Attributes serve various functions. They are used to annotate, optimize code generation or improve diagnostics.
In general, the compiler is allowed to ignore attributes.
They are permitted to observably affect the execution, the code must not rely on such side effects though.

## Syntax

    #name
    #name(parameter)
    #name(parameter, parameter)

* there is no space between `#` character and attribute name
* name
* parameter ??? do any exist ??? parentheses would introduce significant whitespace
* attribute is terminated by first white-space or a semi-colon character not part of attribute's parameter

## Semantics

* after a thing they affect
* typically at the end of the row, after the the whole statement the affect
* user-defined

## [Source code file character set](charset.md)

    #UTF-8

Case-insensitive, changes how the source code file data are interpreted immediately following the terminating semicolon.

## TBD

    #uninitialized // keep stack trash
    #deferred // evaluation may/should be deferred to any point before first use
    #ignore-exceptions // any thrown exception is caught and ignored

...

