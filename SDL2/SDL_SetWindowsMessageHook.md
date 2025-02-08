# SDL_SetWindowsMessageHook

Set a callback for every Windows message, run before TranslateMessage().

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
void SDL_SetWindowsMessageHook(SDL_WindowsMessageHook callback, void *userdata);
```

## Function Parameters

|                                                  |              |                                                                        |
| ------------------------------------------------ | ------------ | ---------------------------------------------------------------------- |
| [SDL_WindowsMessageHook](SDL_WindowsMessageHook) | **callback** | The [SDL_WindowsMessageHook](SDL_WindowsMessageHook) function to call. |
| void *                                           | **userdata** | a pointer to pass to every iteration of `callback`.                    |

## Version

This function is available since SDL 2.0.4.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

