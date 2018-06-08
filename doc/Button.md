### `Button`:

Corresponds to:
[`Fl_Button`](http://www.fltk.org/doc-1.3/classFl__Button.html)

Inherits from:
[`Widget`](Widget)

*   `fl.Button( i, i, i, i, ns ) ==> u`
*   `fl.Button( t ) ==> u` (table constructor syntax)
*   `obj:clear() ==> b`
*   `obj:set() ==> b`
*   `obj:setonly()`
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.type  [get: s; set: s]`
*   `obj.value  [get: b; set: b]`
*   `obj.down_box  [get: s; set: s]`
*   `obj.shortcut  [get: u; set: isu]`
*   `obj.down_color  [get: u; set: iu]`
*   properties defined for the [`Widget`](Widget) userdata type

Different behavior for the button can be selected by setting its
`type` property to one of:

*   `"FL_NORMAL_BUTTON"` (the default)
*   `"FL_TOGGLE_BUTTON"`
*   `"FL_RADIO_BUTTON"`

