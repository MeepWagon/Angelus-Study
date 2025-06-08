# Why use a build system?
Incremental builds. In a large code base, with thousands of lines of code, it can take long periods of time to compile every code file. A build system tracks code file and dependency changes, so that if any file has changed since compiling the last time, it will then be recompiled. If it hasn't changed since the last compile, it will just use the cached object file.
# Tools
- Crosstool-NG: A tool for building cross-platform tool chains.
- Meson: Build system generator. Modern alternative to CMake.
- Ninja: Build system.
- Make: Build system.
- CMake: Build system generator. Mostly used with legacy C/C++ code.
- Premake: Build system generator. Modern alternative to CMake (?)
- Autotools: Build system generator, part of the GNU build system.
- Visual Studio: Full IDE. Includes:
	- Debugger
	- Read more on what visual studio does. (Low priority)

