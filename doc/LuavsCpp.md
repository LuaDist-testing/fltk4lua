## Differences Lua API vs. C++ API

In general there are the following differences between Lua API and C++
API (assuming you did a `local fl = require( "fltk4lua" )` at the top
of your Lua source file):

*   The prefixes of classes and functions have been removed, so use
    *   `fl.message()` instead of `fl_message()`
    *   `fl.run()` instead of `Fl::run()`
    *   `fl.Box()` instead of `new Fl_Box()`
    *   `fl.ALIGN_CENTER` instead of `FL_ALIGN_CENTER` (but see below).
*   Some `enum`s or preprocessor macros are translated to strings:
    *   `"FL_UP_BOX"` instead of `FL_UP_BOX`.
*   The remaining `enum`s/macros are available as userdata, so that
    you can combine them using bitwise operators (in Lua 5.3) or the
    following alternative operators:
    *   `local a = fl.ALIGN_TOP + fl.ALIGN_LEFT` instead of
        `Fl_Align a = FL_ALIGN_TOP | FL_ALIGN_LEFT;`
    *   `local a = b - fl.ALIGN_LEFT` instead of
        `Fl_Align a = b & (~FL_ALIGN_LEFT);` and
    *   `if a( fl.ALIGN_TOP ) then` instead of `if( a & FL_ALIGN_TOP )`
        (more specifically it's `!(~a & FL_ALIGN_TOP)`, but that only
        matters when multiple bits are set in the right-hand-side).
*   C++ method calls are translated to Lua properties whenever
    possible, so use
    *   `b.box = "FL_UP_BOX"` instead of `b->box( FL_UP_BOX );` and
    *   `local bt = b.box` instead of `Fl_Boxtype bt = b->box();`.
*   Integers used as boolean values are translated to real `boolean`s.
*   `nil` is translated to `NULL` if `NULL` is allowed (and vice
    versa).
*   Output parameters end up as (multiple) return values.
*   The menu interface is a bit different, though, as it is completely
    index based, and the `Fl_Menu_Item`s are not exposed as userdata.
    Instead there are extra methods on the widget that contains the
    menu items.

