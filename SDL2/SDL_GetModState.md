# SDL_GetModState

Get the current key modifier state for the keyboard.

## Header File

Defined in [SDL_keyboard.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_keyboard.h)

## Syntax

```c
SDL_Keymod SDL_GetModState(void);
```

## Return Value

([SDL_Keymod](SDL_Keymod)) Returns an OR'd combination of the modifier keys
for the keyboard. See [SDL_Keymod](SDL_Keymod) for details.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetKeyboardState](SDL_GetKeyboardState)
- [SDL_SetModState](SDL_SetModState)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

