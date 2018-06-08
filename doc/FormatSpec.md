## Interface Format Spec

The function/property prototypes are listed using the following
format:

*   The parameter types of function calls are declared inside the
    parentheses after the function name.
*   Return value types for functions are specified after `==>`.
*   The types listed for properties indicate the return value for the
    `__index` metamethod (`get:` part), or the required value type
    for the `__newindex` metamethod (`set:` part). The only valid type
    for keys is `string` for both metamethods. A dash (`-`) means that
    the property can't be read/written (but an inherited property of
    the same name might be used instead).
*   Lua types are abbreviated as:  `nil=n`, `boolean=b`, `integer=i`,
    `number=d` (think `double`), `string=s`, `function=f`,
    `userdata=u`, `coroutine=c`, `table=t`, `any (non-nil)=a`.
    Alternative types are concatenated together, so e.g.  `nu` means
    `nil` or `userdata`.
*   Parameters at the end of the parameter list which also accept
    `nil` can be left out as usual (optional parameters).
*   Boolean parameters accept any Lua value (interpreted as
    true-ish/false-y as usual), so a boolean parameter at the end of
    the parameter list is optional as well.
*   There are a few exceptions where the number of arguments is used
    to select an overloaded C++ method, but those cases are rare.
    Usually such functions are listed multiple times with different
    prototypes.
*   Sometimes (groups of) optional arguments are explicitly marked
    using square brackets. In such a case you should provide none or
    all of the optional arguments.

If a function and a property have the same name, the function always
takes precedence (hopefully the affected function or the property has
been renamed to avoid this case), and methods/properties defined on
the sub-class take precedence over inherited ones.

