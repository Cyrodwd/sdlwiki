# SDL_SetWindowPosition

Set the position of a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void SDL_SetWindowPosition(SDL_Window * window,
                           int x, int y);
```

## Function Parameters

|                            |            |                                                                                                                                                                      |
| -------------------------- | ---------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to reposition.                                                                                                                                            |
| int                        | **x**      | the x coordinate of the window in screen coordinates, or [`SDL_WINDOWPOS_CENTERED`](SDL_WINDOWPOS_CENTERED) or [`SDL_WINDOWPOS_UNDEFINED`](SDL_WINDOWPOS_UNDEFINED). |
| int                        | **y**      | the y coordinate of the window in screen coordinates, or [`SDL_WINDOWPOS_CENTERED`](SDL_WINDOWPOS_CENTERED) or [`SDL_WINDOWPOS_UNDEFINED`](SDL_WINDOWPOS_UNDEFINED). |

## Remarks

The window coordinate origin is the upper left of the display.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetWindowPosition](SDL_GetWindowPosition)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

