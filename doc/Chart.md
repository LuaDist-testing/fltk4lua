### `Chart`:

Corresponds to:
[`Fl_Chart`](http://www.fltk.org/doc-1.3/classFl__Chart.html)

Inherits from:
[`Widget`](Widget)

*   `fl.Chart( i, i, i, i, ns ) ==> u`
*   `fl.Chart( t ) ==> u` (table constructor syntax)
*   `obj:add( d, ns, niu )`
*   `obj:bounds() ==> d, d`
*   `obj:bounds( d, d )`
*   `obj:clear()`
*   `obj:insert( i, d, ns, niu )`
*   `obj:replace( i, d, ns, niu )`
*   `obj:size( i, i )`
*   methods defined for the [`Widget`](Widget) userdata type
*   `obj.type  [get: s; set: s]`
*   `obj.maxsize  [get: i; set: i]`
*   `obj.autosize  [get: b; set: b]`
*   `obj.textsize  [get: i; set: i]`
*   `obj.textcolor  [get: u; set: iu]`
*   `obj.chart_size  [get: i; set: -]` (corresponds to
    `Fl_Chart::size()`)
*   properties defined for the [`Widget`](Widget) userdata type

The `type` property of charts can be set to one of the following
values:

*   `"FL_BAR_CHART"`
*   `"FL_FILLED_CHART"`
*   `"FL_HORBAR_CHART"`
*   `"FL_LINE_CHART"`
*   `"FL_PIE_CHART"`
*   `"FL_SPECIALPIE_CHART"`
*   `"FL_SPIKE_CHART"`

