### `Spinner`:

Corresponds to:
[`Fl_Spinner`](http://www.fltk.org/doc-1.3/classFl__Spinner.html)

Inherits from:
[`Widget`](Widget)

*   `fl.Spinner( i, i, i, i, ns ) ==> u`
*   `fl.Spinner( t ) ==> u` (table constructor syntax)
*   `obj:range( d, d )`
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.step  [get: d; set: d]`
*   `obj.type  [get: s; set: s]`
*   `obj.color  [get: u; set: iu]`
*   `obj.value  [get: d; set: d]`
*   `obj.format  [get: s; set: s]`
*   `obj.maximum  [get: d; set: d]`
*   `obj.minimum  [get: d; set: d]`
*   `obj.textfont  [get: s; set: is]`
*   `obj.textsize  [get: i; set: i]`
*   `obj.textcolor  [get: u; set: iu]`
*   properties defined for the [`Widget`](Widget) userdata type

(note: `Spinner` does not inherit the methods and properties of
`Group`, although `Fl_Spinner` is implemented as a sub-class of
`Fl_Group`!)

The `type` property of spinner widgets can be set to one of the
following values:

*   `"FL_INT_INPUT"`
*   `"FL_FLOAT_INPUT"`

