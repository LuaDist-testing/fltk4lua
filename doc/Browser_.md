### `Browser_` (abstract):

Corresponds to:
[`Fl_Browser_`](http://www.fltk.org/doc-1.3/classFl__Browser__.html)

*   `obj:deselect( b ) ==> b`
*   `obj:scrollbar_left()`
*   `obj:scrollbar_right()`
*   `obj:sort( ns )`
*   `obj.textfont  [get: s; set: is]`
*   `obj.textsize  [get: i; set: i]`
*   `obj.textcolor  [get: u; set: iu]`
*   `obj.hposition  [get: i; set: i]`
*   `obj.vposition  [get: i; set: i]` (corresponds to
    `Fl_Browser_::position()`)
*   `obj.has_scrollbar  [get: s; set: s]`
*   `obj.scrollbar_size  [get: i; set: i]`
*   `obj.scrollbar_width  [get: i; set: i]`

The `has_scrollbar` property of browser widgets can be set to one of
the following values to select which scrollbars are shown:

*   `"HORIZONTAL"`
*   `"VERTICAL"`
*   `"BOTH"` (the default)
*   `"HORIZONTAL_ALWAYS"`
*   `"VERTICAL_ALWAYS"`
*   `"BOTH_ALWAYS"`

