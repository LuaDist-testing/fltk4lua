### `Input`:

Corresponds to:
[`Fl_Input`](http://www.fltk.org/doc-1.3/classFl__Input.html),
[`Fl_Input_`](http://www.fltk.org/doc-1.3/classFl__Input__.html)

Inherits from:
[`Widget`](Widget)

*   `fl.Input( i, i, i, i, ns ) ==> u`
*   `fl.Input( t ) ==> u` (table constructor syntax)
*   `obj:copy( i ) ==> b`
*   `obj:copy_cuts() ==> b`
*   `obj:cut( [i [, i]] ) ==> b`
*   `obj:index( i ) ==> i`
*   `obj:insert( s ) ==> b`
*   `obj:replace( i, i, ns ) ==> b`
*   `obj:size( i, i )`
*   `obj:undo()`
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.mark  [get: i; set: i]`
*   `obj.type  [get: s; set: s]`
*   `obj.wrap  [get: b; set: b]`
*   `obj.value  [get: s; set: s]`
*   `obj.tab_nav  [get: b; set: b]`
*   `obj.readonly  [get: b; set: b]`
*   `obj.shortcut  [get: u; set: isu]`
*   `obj.textfont  [get: s; set: is]`
*   `obj.textsize  [get: i; set: i]`
*   `obj.textcolor  [get: u; set: iu]`
*   `obj.value_size  [get: i; set: -]` (corresponds to
    `Fl_Input_::size()`)
*   `obj.cursor_color  [get: u; set: iu]`
*   `obj.maximum_size  [get: i; set: i]`
*   `obj.cursor_position  [get: i; set: i]` (corresponds to
    `Fl_Input_::position(int [, int])`)
*   properties defined for the [`Widget`](Widget) userdata type

The `type` property of input widgets can be set to one of the
following values:

*   `"FL_NORMAL_INPUT"` (the default)
*   `"FL_FLOAT_INPUT"`
*   `"FL_INT_INPUT"`
*   `"FL_HIDDEN_INPUT"`
*   `"FL_MULTILINE_INPUT"`
*   `"FL_SECRET_INPUT"`
*   `"FL_NORMAL_OUTPUT"`
*   `"FL_MULTILINE_OUTPUT"`
*   `"FL_MULTILINE_INPUT_WRAP"`
*   `"FL_MULTILINE_OUTPUT_WRAP"`

