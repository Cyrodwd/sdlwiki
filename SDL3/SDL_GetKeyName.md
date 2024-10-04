###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetKeyName

Get a human-readable name for a key.

## Header File

Defined in [<SDL3/SDL_keyboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_keyboard.h)

## Syntax

```c
const char * SDL_GetKeyName(SDL_Keycode key);
```

## Function Parameters

|                            |         |                                                  |
| -------------------------- | ------- | ------------------------------------------------ |
| [SDL_Keycode](SDL_Keycode) | **key** | the desired [SDL_Keycode](SDL_Keycode) to query. |

## Return Value

(const char *) Returns a UTF-8 encoded string of the key name.

## Remarks

If the key doesn't have a name, this function returns an empty string ("").

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetKeyFromName](SDL_GetKeyFromName)
- [SDL_GetKeyFromScancode](SDL_GetKeyFromScancode)
- [SDL_GetScancodeFromKey](SDL_GetScancodeFromKey)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

