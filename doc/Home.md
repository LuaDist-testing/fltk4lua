# fltk4lua -- Lua Binding to the Fast Light Tool Kit

[FLTK][1] is a small C++ GUI toolkit portable to the MS Windows,
Linux, and Mac OSX operating systems. **fltk4lua** is a binding to
this C++ toolkit, which allows you to create GUIs from within Lua
scripts.

**fltk4lua** is available via the [LuaRocks package manager][2]. For
details about building/installing the module see [here](Building).

Although FLTK is a small GUI toolkit, it still has many classes and
functions. **fltk4lua** currently exports more than 50 different
userdata types and hundreds of C++ functions. Fortunately the Lua API
is [very close to the C++ API](LuavsCpp), so you can use the
[official FLTK documentation][3], and look at the Lua examples in the
repository, or at the source code. There is also a [Getting Started
Guide](GettingStarted), which builds a simple GUI with **fltk4lua**
and explains every step.

  [1]:  http://www.fltk.org/
  [2]:  http://luarocks.org/
  [3]:  http://www.fltk.org/doc-1.3/index.html

However, here is a list of userdata types/functions/properties that
are available in Lua. The format of the listing (especially the
function prototypes) is specified [here](FormatSpec).

*   [`Image` (abstract)](Image)
*   [`Shared_Image`](Shared_Image)
*   [`Widget` (abstract)](Widget)
*   [`Box`](Box)
*   [`Button`](Button)
*   [`Light_Button`](Light_Button)
*   [`Check_Button`](Check_Button)
*   [`Repeat_Button`](Repeat_Button)
*   [`Return_Button`](Return_Button)
*   [`Round_Button`](Round_Button)
*   [`Chart`](Chart)
*   [`Clock_Output`](Clock_Output)
*   [`Clock`](Clock)
*   [`Group`](Group)
*   [`Browser_` (abstract)](Browser_)
*   [`Browser`](Browser)
*   [`File_Browser`](File_Browser)
*   [`Check_Browser`](Check_Browser)
*   [`Color_Chooser`](Color_Chooser)
*   [`Input_Choice`](Input_Choice)
*   [`Pack`](Pack)
*   [`Scroll`](Scroll)
*   [`Spinner`](Spinner)
*   [`Tabs`](Tabs)
*   [`Tile`](Tile)
*   [`Window`](Window)
*   [`Wizard`](Wizard)
*   [`Input`](Input)
*   [`File_Input`](File_Input)
*   [`Menu` (abstract)](Menu)
*   [`Choice`](Choice)
*   [`Menu_Bar`](Menu_Bar)
*   [`Menu_Button`](Menu_Button)
*   [`Progress`](Progress)
*   [`Valuator` (abstract)](Valuator)
*   [`Adjuster`](Adjuster)
*   [`Counter`](Counter)
*   [`Dial`](Dial)
*   [`Roller`](Roller)
*   [`Slider`](Slider)
*   [`Scrollbar`](Scrollbar)
*   [`Value_Slider`](Value_Slider)
*   [`Value_Input`](Value_Input)
*   [`Value_Output`](Value_Output)
*   [additional module functions](Functions)

