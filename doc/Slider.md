### `Slider`:

Corresponds to:
[`Fl_Slider`](http://www.fltk.org/doc-1.3/classFl__Slider.html)

Inherits from:
[`Valuator`](Valuator),
[`Widget`](Widget)

*   `fl.Slider( i, i, i, i, ns ) ==> u`
*   `fl.Slider( t ) ==> u` (table constructor syntax)
*   `obj:bounds( d, d )`
*   `obj:scrollvalue( i, i, i, i ) ==> i`
*   methods defined for the [`Valuator`](Valuator) userdata type
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.type  [get: s; set: s]`
*   `obj.slider  [get: s; set: s]`
*   `obj.slider_size  [get: d; set: d]`
*   properties defined for the [`Valuator`](Valuator) userdata type
*   properties defined for the [`Widget`](Widget) userdata type

The `type` property of slider widgets can be set to one of the
following values:

*   `"FL_VERTICAL"`
*   `"FL_HORIZONTAL"`
*   `"FL_VERT_FILL_SLIDER"`
*   `"FL_HOR_FILL_SLIDER"`
*   `"FL_VERT_NICE_SLIDER"`
*   `"FL_HOR_NICE_SLIDER"`

