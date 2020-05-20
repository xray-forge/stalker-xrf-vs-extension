# C++ Debugger Extensions for Lua

---
This Visual Studio extension enables limited support for inspection of Lua (Version 5.3) state in C++ applications during debug.

## Features:
 * Lua 'inline' stack frame insertion into the Call Stack
 * Mark Lua library stack frames as non-user code
 * Jump to Lua source/line from Lua stack frames
 * Function argument and local variable display in the 'Locals' watch section
 * Local variable lookup in Watch, Immediate and similar elements

 ## Known Issues:
 * This extension will always add Lua module to the application (can be seen in 'Modules' section of the debugger) even when debugging applications with no Lua code (check notes in RemoteComponent.cs)
 * Lua source files are located based on the process working directory, additional configuration options are planned in the future
