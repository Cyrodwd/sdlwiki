###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetModState

Get the current key modifier state for the keyboard.

## Header File

Defined in [<SDL3/SDL_keyboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_keyboard.h)

## Syntax

```c
SDL_Keymod SDL_GetModState(void);
```

## Return Value

([SDL_Keymod](SDL_Keymod)) Returns an OR'd combination of the modifier keys
for the keyboard. See [SDL_Keymod](SDL_Keymod) for details.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetKeyboardState](SDL_GetKeyboardState)
- [SDL_SetModState](SDL_SetModState)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

