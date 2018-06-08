### `Menu_Button`:

Corresponds to:
[`Fl_Menu_Button`](http://www.fltk.org/doc-1.3/classFl__Menu__Button.html)

Inherits from:
[`Menu`](Menu),
[`Widget`](Widget)

*   `fl.Menu_Button( i, i, i, i, ns ) ==> u`
*   `fl.Menu_Button( t ) ==> u` (table constructor syntax)
*   methods defined for the [`Menu`](Menu) userdata type
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.type  [get: s; set: s]`
*   properties defined for the [`Menu`](Menu) userdata type
*   properties defined for the [`Widget`](Widget) userdata type

The `type` property of menu button widgets can be set to one of the
following values to select the mouse button(s) that activate the menu:

*   `"NOPOPUP"`
*   `"POPUP1"`
*   `"POPUP2"`
*   `"POPUP12"`
*   `"POPUP3"` (usually what you want)
*   `"POPUP13"`
*   `"POPUP23"`
*   `"POPUP123"`

