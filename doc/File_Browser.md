### `File_Browser`:

Corresponds to:
[`Fl_File_Browser`](http://www.fltk.org/doc-1.3/classFl__File__Browser.html)

Inherits from:
[`Browser`](Browser),
[`Browser_`](Browser_),
[`Widget`](Widget)

*   `fl.File_Browser( i, i, i, i, ns ) ==> u`
*   `fl.File_Browser( t ) ==> u` (table constructor syntax)
*   `obj:load( s, s ) ==> b / (n, s, i)`
*   methods defined for the [`Browser`](Browser) userdata type
*   methods defined for the [`Browser_`](Browser_) userdata type
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.filter  [get: s; set: s]`
*   `obj.filetype  [get: s; set: s]`
*   `obj.iconsize  [get: i; set: i]`
*   `obj.textsize  [get: i; set: i]`
*   properties defined for the [`Browser`](Browser) userdata type
*   properties defined for the [`Browser_`](Browser_) userdata type
*   properties defined for the [`Widget`](Widget) userdata type

(note: `File_Browser` does not inherit the methods and properties of
`Group`, although `Fl_File_Browser` is implemented as a sub-class of
`Fl_Group`!)

The `filetype` property of file browsers can be set to one of the
following values:

*   `"FILES"`
*   `"DIRECTORIES"`

