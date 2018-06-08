##                        Building/Installing                       ##

**fltk4lua** is compatible with Lua 5.1 (including LuaJIT), 5.2, and
5.3, for which the required include files have to be available. You
will also need a C/C++ compiler (yes, one that actually can do both)
and FLTK version 1.3 installed. On Unixes you can probably use the
package manager for that (on Debian/Ubuntu it's `libfltk1.3-dev`, in
Homebrew it's plain `fltk`). On Windows you will need to compile FLTK
yourself (I have had success for both MinGW and MSVC++ Express 2010
using CMAKE).

The supplied Makefile is configured for Lua 5.2 on a Debian/Ubuntu
Linux system. For other Unixes or other Lua installs you will have to
change some variables in the Makefile (in particular `DLL_INSTALL_DIR`
and `LUA_INCDIR` near the top -- most other compilation settings are
determined by calling `fltk-config`) unless you build using LuaRocks
which will do that for you automatically. For Windows the only
supported way of building **fltk4lua** is via [LuaRocks][1].

  [1]:  http://luarocks.org/


###           Installing the latest release via LuaRocks           ###

On Unix with FLTK installed system-wide a

    luarocks install fltk4lua

should do the trick. On Windows you will probably have to specify the
locations of FLTK header files and libraries:

    luarocks install fltk4lua \
        FLTK_INCDIR=/path/to/FL/incdir FLTK_LIBDIR=/path/to/fltk/libs

If you are building on Windows for Lua 5.3, you will also need to
install an updated `luarocks-build-cpp` rock, because the one in the
main LuaRocks repository (version 0.1 at the time of this writing) is
not compatible with Lua 5.3. You can find a working fork [here on
GitHub][2], or in a separate manifest in the LuaRocks repository:

    luarocks install --server=http://luarocks.org/manifests/siffiejoe \
        luarocks-build-cpp

  [2]:  https://github.com/siffiejoe/luarocks-build-cpp


###         Installing the development version via LuaRocks        ###

To install the latest version of **fltk4lua** from GitHub you just
clone the repository *recursively* and run `luarocks make`:

    git clone https://github.com/siffiejoe/lua-fltk4lua --recursive
    cd lua-fltk4lua
    luarocks make

(On Windows don't forget to specify `FLTK_INCDIR` and `FLTK_LIBDIR`!)

Or you just use the dev manifest when invoking LuaRocks:

    luarocks install --server=http://luarocks.org/dev fltk4lua

However, you will need a `git` executable installed that LuaRocks can
use (this is usually not a problem on Unix).

