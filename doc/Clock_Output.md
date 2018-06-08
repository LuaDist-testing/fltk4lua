### `Clock_Output`:

Corresponds to:
[`Fl_Clock_Output`](http://www.fltk.org/doc-1.3/classFl__Clock__Output.html)

Inherits from:
[`Widget`](Widget)

*   `fl.Clock_Output( i, i, i, i, ns ) ==> u`
*   `fl.Clock_Output( t ) ==> u` (table constructor syntax)
*   `obj:setvalue( i, i, i )` (corresponds to
    `Fl_Clock_Output::value(int, int, int)`)
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.hour  [get: i; set: -]`
*   `obj.type  [get: s; set: s]`
*   `obj.value  [get: id; set: id]` (type depends on size of
    `lua_Integer`)
*   `obj.minute  [get: i; set: -]`
*   `obj.second  [get: i; set: -]`
*   properties defined for the [`Widget`](Widget) userdata type

The `type` property of the clock (output) can be set to one of the
following values:

*   `"FL_SQUARE_CLOCK"` (the default)
*   `"FL_ROUND_CLOCK"`

