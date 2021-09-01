# Programming Language
*Modern systems programming language design experiment*

## Hello World!

    #utf-8
    
    import std:io;
    import "user32.dll" "MessageBeep" MessageBeep
    import "user32.dll" "MessageBoxW"
    
    define main : ¶word:32 {
        const msg = "Hello World!";
    
        routine:
            std:io:print (msg "\n");
            MessageBeep (0);
            return user32.dll!MessageBoxW (null, msg:ucs16, "Hi":ucs16, 0u:32);
    }

*note that example above is subject to significant changes*

## Discussion
...remove main causes of user errors

TODO:
* name discussion, goals of the effort
* semantics differences, clean-slate C++? runtime? requirements and limitations? calling conventions? visual studio integration

## Language reference
* [Text file](charset.md), [Comments](comments.md), Keywords, Identifiers,
* Literals, [Attributes](attributes.md), [Types/Declarations](types.md), Definitions, Expressions, Flow control
* [Reflection](reflection.md), Objects/Functions, Templates, Modules, Programs
* Translation

## Execution environment
## Libraries

