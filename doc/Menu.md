### `Menu` (abstract):

Corresponds to:
[`Fl_Menu_`](http://www.fltk.org/doc-1.3/classFl__Menu__.html),
[`Fl_Menu_Item`](http://www.fltk.org/doc-1.3/structFl__Menu__Item.html)

*   `obj:add( s, nisu, nf, na, nu ) ==> i`
*   `obj:clear()`
*   `obj:clear_submenu( i ) ==> nb`
*   `obj:find_index( s ) ==> ni`
*   `obj:insert( i, s, nisu, nf, na, nu ) ==> i`
*   `obj:remove( i )`
*   `obj:size( i, i )`
*   `obj:menuitem_getp( i, s ) ==> ?` gets a property value for the
    menu element identified by the given index.
    -   `"text" ==> ns`
    -   `"flags" ==> u`
    -   `"label" ==> ns`
    -   `"callback" ==> nf`
    -   `"shortcut" ==> u`
    -   `"labelfont" ==> s`
    -   `"labelsize" ==> i`
    -   `"labeltype" ==> s`
    -   `"user_data" ==> na`
    -   `"labelcolor" ==> u`
*   `obj:menuitem_setp( i, s, ? )`
    -   `"text": s`
    -   `"flags": u`
    -   `"label": s`
    -   `"callback": nf`
    -   `"shortcut": isu`
    -   `"labelfont": is`
    -   `"labelsize": i`
    -   `"labeltype": s`
    -   `"user_data": na`
    -   `"labelcolor": iu`
*   `obj:menuitem_activate( i )`
*   `obj:menuitem_active( i ) ==> b`
*   `obj:menuitem_activevisible( i ) ==> b`
*   `obj:menuitem_checkbox( i ) ==> b`
*   `obj:menuitem_clear( i )`
*   `obj:menuitem_deactivate( i )`
*   `obj:menuitem_hide( i )`
*   `obj:menuitem_radio( i ) ==> b`
*   `obj:menuitem_set( i )`
*   `obj:menuitem_setonly( i )`
*   `obj:menuitem_show( i )`
*   `obj:menuitem_submenu( i ) ==> b`
*   `obj:menuitem_value( i ) ==> b`
*   `obj:menuitem_visible( i ) ==> b`
*   `obj.value  [get: i; set: i]`
*   `obj.down_box  [get: s; set: s]`
*   `obj.textfont  [get: s; set: is]`
*   `obj.textsize  [get: i; set: i]`
*   `obj.menu_size  [get: i; set: -]`
*   `obj.textcolor  [get: u; set: iu]`

