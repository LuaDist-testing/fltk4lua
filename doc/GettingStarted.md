## Getting Started

**fltk4lua** consists of a single C module that you can load via
`require`:

    local fl = require( "fltk4lua" )

FLTK is a GUI toolkit with its own event loop, which you can run using
the `fl.run()` method. This method will process all events until the
last [Window](Window) becomes hidden. This is also the preferred way
of exiting an FLTK application.

    local fl = require( "fltk4lua" )
    fl.run()  -- will return immediately, because there is no window

In addition to `fl.run()` there are functions that only handle a small
amout of events (`fl.wait()` and `fl.check()`), so that you can
integrate the FLTK event loop with some other event loop.

For the application to show a GUI, you need to create and `show()` a
window:

    local fl = require( "fltk4lua" )
    local window = fl.Window( 340, 180, "Hello" )
    window:show( arg )  -- process certain command line flags
    fl.run()

The `fl.Window()` constructor takes the width and the height of the
window in pixels, as well as an optional title as a string, and returns
a window object.  Since the window is `show()`n, the `fl.run()` method
will handle events until the window becomes invisible again. FLTK by
default hides the current window when you press `ESC`, so this is one
way to quit the example program above.

All windows are derived from [Group](Group), which means that they can
contain child widgets. All widgets are automatically added to the last
group object created until you call the `end_group()` method on the
group object.

    local fl = require( "fltk4lua" )
    local window = fl.Window( 340, 180, "Hello" )
    local box = fl.Box( 20, 40, 300, 100, "Hello World!" )
    window:end_group()
    window:show( arg )
    fl.run()

The constructors of all [Widget](Widget)s take the same arguments: the
x and y coordinates of the top left corner, the width and height in
pixels, and an optional label. In fact, since windows are regular
widgets, the window constructor will accept those arguments as well. A
[Box](Box) is one of the simplest widgets in FLTK. It is used only for
visual effect:

    local fl = require( "fltk4lua" )
    local window = fl.Window( 340, 180, "Hello" )
    local box = fl.Box( 20, 40, 300, 100, "Hello World!" )
    box.box = "FL_UP_BOX"
    box.labelfont = "FL_HELVETICA_BOLD_ITALIC"
    box.labelsize = 36
    box.labeltype = "FL_SHADOW_LABEL"
    window:end_group()
    window:show( arg )
    fl.run()

There is some syntax sugar for widget constructors which allows you to
specify properties directly when creating the widget. And since
widgets are added to the parent group automatically, you sometimes
don't even need a variable for the widget object:

    local fl = require( "fltk4lua" )
    local window = fl.Window( 340, 180, "Hello" )
    fl.Box{ 20, 40, 300, 100, "Hello World!",
      box = "FL_UP_BOX", labelfont = "FL_HELVETICA_BOLD_ITALIC",
      labelsize = 36, labeltype = "FL_SHADOW_LABEL"
    }
    window:end_group()
    window:show( arg )
    fl.run()

When something important happens with the GUI (like a button press
for instance), FLTK will call a callback function on the target
widget, passing the widget as first argument and a `user_data` value
as the second argument (FLTK calls it `user_data`, it doesn't have to
be a Lua userdata). Of course you can use a closure to have access to
any Lua value in a local variable ...

    local fl = require( "fltk4lua" )
    local window = fl.Window( 340, 210, "Hello" )
    fl.Box{ 20, 40, 300, 100, "Hello World!",
      box = "FL_UP_BOX", labelfont = "FL_HELVETICA_BOLD_ITALIC",
      labelsize = 36, labeltype = "FL_SHADOW_LABEL"
    }
    fl.Button{ 20, 150, 140, 30, "Print Me",
      user_data = "some Lua value", callback = print
    }
    local btn = fl.Button( 180, 150, 140, 30, "Quit" )
    function btn:callback()
      window:hide()  -- will cleanly exit the application
    end
    window:end_group()
    window:show( arg )
    fl.run()

This should get you started. You can take a look at the [list of
widgets](Home) **fltk4lua** provides you with, and the properties and
methods you can use.

Have fun!

