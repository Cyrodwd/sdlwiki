# SDL_GetWindowPosition

Get the position of a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void SDL_GetWindowPosition(SDL_Window * window,
                           int *x, int *y);
```

## Function Parameters

|                            |            |                                                                                            |
| -------------------------- | ---------- | ------------------------------------------------------------------------------------------ |
| [SDL_Window](SDL_Window) * | **window** | the window to query.                                                                       |
| int *                      | **x**      | a pointer filled in with the x position of the window, in screen coordinates, may be NULL. |
| int *                      | **y**      | a pointer filled in with the y position of the window, in screen coordinates, may be NULL. |

## Remarks

If you do not need the value for one of the positions a NULL may be passed
in the `x` or `y` parameter.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetWindowPosition](SDL_SetWindowPosition)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

