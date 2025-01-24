# SDL_WarpMouseInWindow

Move the mouse cursor to the given position within the window.

## Header File

Defined in [SDL_mouse.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mouse.h)

## Syntax

```c
void SDL_WarpMouseInWindow(SDL_Window * window,
                           int x, int y);
```

## Function Parameters

|                            |            |                                                                         |
| -------------------------- | ---------- | ----------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to move the mouse into, or NULL for the current mouse focus. |
| int                        | **x**      | the x coordinate within the window.                                     |
| int                        | **y**      | the y coordinate within the window.                                     |

## Remarks

This function generates a mouse motion event if relative mode is not
enabled. If relative mode is enabled, you can force mouse events for the
warp by setting the
[SDL_HINT_MOUSE_RELATIVE_WARP_MOTION](SDL_HINT_MOUSE_RELATIVE_WARP_MOTION)
hint.

Note that this function will appear to succeed, but not actually move the
mouse when used over Microsoft Remote Desktop.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_WarpMouseGlobal](SDL_WarpMouseGlobal)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMouse](CategoryMouse)

