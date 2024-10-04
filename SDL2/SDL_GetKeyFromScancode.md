###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetKeyFromScancode

Get the key code corresponding to the given scancode according to the current keyboard layout.

## Header File

Defined in [SDL_keyboard.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_keyboard.h)

## Syntax

```c
SDL_Keycode SDL_GetKeyFromScancode(SDL_Scancode scancode);
```

## Function Parameters

|                              |              |                                                    |
| ---------------------------- | ------------ | -------------------------------------------------- |
| [SDL_Scancode](SDL_Scancode) | **scancode** | the desired [SDL_Scancode](SDL_Scancode) to query. |

## Return Value

([SDL_Keycode](SDL_Keycode)) Returns the [SDL_Keycode](SDL_Keycode) that
corresponds to the given [SDL_Scancode](SDL_Scancode).

## Remarks

See [SDL_Keycode](SDL_Keycode) for details.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetKeyName](SDL_GetKeyName)
- [SDL_GetScancodeFromKey](SDL_GetScancodeFromKey)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

