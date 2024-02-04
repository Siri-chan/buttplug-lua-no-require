# buttplug.lua

This is a [buttplug.io](buttplug.io) client written in Lua.

## Features

- Seamless device connects/disconnects

## Example code

TODO

## Known issues

- Does not handle multiple devices

## But why without `require`???
so as it turns out, when using `require` in payday 2, BLT overwrites it. this would be fine, but it also changes the root path of require and causes an error:
```
about to perform blocking dns call from the main thread. consider refactoring.
```
so, to work with this within payday 2, I need my own fucky versions of require, using loadstring.
THIS WILL NOT WORK ABOVE LUA 5.1
