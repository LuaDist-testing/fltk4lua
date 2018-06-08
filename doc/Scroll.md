### `Scroll`:

Corresponds to:
[`Fl_Scroll`](http://www.fltk.org/doc-1.3/classFl__Scroll.html)

Inherits from:
[`Group`](Group),
[`Widget`](Widget)

*   `fl.Scroll( i, i, i, i, ns ) ==> u`
*   `fl.Scroll( t ) ==> u` (table constructor syntax)
*   `obj:clear()`
*   `obj:scroll_to( i, i )`
*   methods defined for the [`Group`](Group) userdata type
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.type  [get: s; set: s]`
*   `obj.scrollbar  [get: u; set: -]`
*   `obj.xposition  [get: i; set: -]`
*   `obj.yposition  [get: i; set: -]`
*   `obj.hscrollbar  [get: u; set: -]`
*   `obj.scrollbar_size  [get: i; set: i]`
*   properties defined for the [`Group`](Group) userdata type
*   properties defined for the [`Widget`](Widget) userdata type

The `type` property of scroll widgets can be set to one of the
folloowing values to select which scrollbar(s) are shown:

*    `"NO_SCROLLBARS"`
*    `"HORIZONTAL"`
*    `"VERTICAL"`
*    `"BOTH"`
*    `"HORIZONTAL_ALWAYS"`
*    `"VERTICAL_ALWAYS"`
*    `"BOTH_ALWAYS"`

