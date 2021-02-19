*Modern systems programming language design experiment*
# Comments

Comment syntax resembles C++ with one major difference: nesting is supported.

## Single line comment

    code;
    // comment
    code;
    code; // comment */ still comment
    code;

## Multi-line comments

    code; /* comment
    comment
    comment */ code;

## Nesting

    code;
    /* comment
        /* nested comment */
        comment
    */
    code;

Single line comment is not considered nested:

    code; /* comment // */ code;

    code; // comment /* comment */ comment

## Ambiguities

...