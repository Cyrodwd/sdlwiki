###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_RunApp

Initializes and launches an SDL application, by doing platform-specific initialization before calling your mainFunction and cleanups after it returns, if that is needed for a specific platform, otherwise it just calls mainFunction.

## Header File

Defined in [<SDL3/SDL_main.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_main.h)

## Syntax

```c
int SDL_RunApp(int argc, char *argv[], SDL_main_func mainFunction, void *reserved);
```

## Function Parameters

|                                |                  |                                                                                                                                            |
| ------------------------------ | ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------ |
| int                            | **argc**         | the argc parameter from the application's main() function, or 0 if the platform's main-equivalent has no argc.                             |
| char **                        | **argv**         | the argv parameter from the application's main() function, or NULL if the platform's main-equivalent has no argv.                          |
| [SDL_main_func](SDL_main_func) | **mainFunction** | your SDL app's C-style main(). NOT the function you're calling this from! Its name doesn't matter; it doesn't literally have to be `main`. |
| void *                         | **reserved**     | should be NULL (reserved for future use, will probably be platform-specific then).                                                         |

## Return Value

(int) Returns the return value from mainFunction: 0 on success, otherwise
failure; [SDL_GetError](SDL_GetError)() might have more information on the
failure.

## Remarks

You can use this if you want to use your own main() implementation without
using [SDL_main](SDL_main) (like when using
[SDL_MAIN_HANDLED](SDL_MAIN_HANDLED)). When using this, you do *not* need
[SDL_SetMainReady](SDL_SetMainReady)().

## Thread Safety

Generally this is called once, near startup, from the process's initial
thread.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMain](CategoryMain)

