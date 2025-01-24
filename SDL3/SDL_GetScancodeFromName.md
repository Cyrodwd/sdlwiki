# SDL_GetScancodeFromName

Get a scancode from a human-readable name.

## Header File

Defined in [<SDL3/SDL_keyboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_keyboard.h)

## Syntax

```c
SDL_Scancode SDL_GetScancodeFromName(const char *name);
```

## Function Parameters

|              |          |                                   |
| ------------ | -------- | --------------------------------- |
| const char * | **name** | the human-readable scancode name. |

## Return Value

([SDL_Scancode](SDL_Scancode)) Returns the [SDL_Scancode](SDL_Scancode), or
[`SDL_SCANCODE_UNKNOWN`](SDL_SCANCODE_UNKNOWN) if the name wasn't
recognized; call [SDL_GetError](SDL_GetError)() for more information.

## Thread Safety

This function is not thread safe.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetKeyFromName](SDL_GetKeyFromName)
- [SDL_GetScancodeFromKey](SDL_GetScancodeFromKey)
- [SDL_GetScancodeName](SDL_GetScancodeName)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

