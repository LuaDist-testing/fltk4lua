### `Browser`:

Corresponds to:
[`Fl_Browser`](http://www.fltk.org/doc-1.3/classFl__Browser.html)

Inherits from:
[`Browser_`](Browser_),
[`Widget`](Widget)

*   `fl.Browser( i, i, i, i, ns ) ==> u`
*   `fl.Browser( t ) ==> u` (table constructor syntax)
*   `obj:add( ns )`
*   `obj:clear()`
*   `obj:displayed( i ) ==> b`
*   `obj:hide( [ i ] )`
*   `obj:insert( i, ns )`
*   `obj:load( s ) ==> b / (n, s, i)`
*   `obj:make_visible( i )`
*   `obj:move( i, i )`
*   `obj:remove( i )`
*   `obj:select( i ) ==> b`
*   `obj:selected( i ) ==> b`
*   `obj:show( [ i ] )`
*   `obj:size( i, i )`
*   `obj:swap( i, i )`
*   `obj:text( i ) ==> ns`
*   `obj:text( i, s )`
*   `obj:line_visible( i ) ==> b` (corresponds to
    `Fl_Browser::visible(int)`)
*   methods defined for the [`Browser_`](Browser_) userdata type
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.type  [get: s; set: s]`
*   `obj.value  [get: i; set: i]`
*   `obj.nitems  [get: i; set: -]` (corresponds to
    `Fl_Browser::size()`)
*   `obj.topline  [get: i; set: i]`
*   `obj.bottomline  [get: -; set: i]`
*   `obj.middleline  [get: -; set: i]`
*   `obj.column_char  [get: s; set: -]`
*   `obj.format_char  [get: s; set: -]`
*   `obj.column_widths  [get: t; set: t]`
*   properties defined for the [`Browser_`](Browser_) userdata type
*   properties defined for the [`Widget`](Widget) userdata type

(note: `Browser` does not inherit the methods and properties of
`Group`, although `Fl_Browser` is implemented as a sub-class of
`Fl_Group`!)

Different behavior for the browser can be selected by setting its
`type` property to one of:

*   `"FL_NORMAL_BROWSER"` (the default)
*   `"FL_SELECT_BROWSER"`
*   `"FL_HOLD_BROWSER"`
*   `"FL_MULTI_BROWSER"`

