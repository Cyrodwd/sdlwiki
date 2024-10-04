###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetKeyFromName

Get a key code from a human-readable name.

## Header File

Defined in [<SDL3/SDL_keyboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_keyboard.h)

## Syntax

```c
SDL_Keycode SDL_GetKeyFromName(const char *name);
```

## Function Parameters

|              |          |                              |
| ------------ | -------- | ---------------------------- |
| const char * | **name** | the human-readable key name. |

## Return Value

([SDL_Keycode](SDL_Keycode)) Returns key code, or
[`SDLK_UNKNOWN`](SDLK_UNKNOWN) if the name wasn't recognized; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetKeyFromScancode](SDL_GetKeyFromScancode)
- [SDL_GetKeyName](SDL_GetKeyName)
- [SDL_GetScancodeFromName](SDL_GetScancodeFromName)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

