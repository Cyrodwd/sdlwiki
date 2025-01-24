# SDL_GetMouseState

Retrieve the current state of the mouse.

## Header File

Defined in [SDL_mouse.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mouse.h)

## Syntax

```c
Uint32 SDL_GetMouseState(int *x, int *y);
```

## Function Parameters

|       |       |                                                                             |
| ----- | ----- | --------------------------------------------------------------------------- |
| int * | **x** | the x coordinate of the mouse cursor position relative to the focus window. |
| int * | **y** | the y coordinate of the mouse cursor position relative to the focus window. |

## Return Value

([Uint32](Uint32)) Returns a 32-bit button bitmask of the current button
state.

## Remarks

The current button state is returned as a button bitmask, which can be
tested using the `SDL_BUTTON(X)` macros (where `X` is generally 1 for the
left, 2 for middle, 3 for the right button), and `x` and `y` are set to the
mouse cursor position relative to the focus window. You can pass NULL for
either `x` or `y`.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetGlobalMouseState](SDL_GetGlobalMouseState)
- [SDL_GetRelativeMouseState](SDL_GetRelativeMouseState)
- [SDL_PumpEvents](SDL_PumpEvents)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMouse](CategoryMouse)

