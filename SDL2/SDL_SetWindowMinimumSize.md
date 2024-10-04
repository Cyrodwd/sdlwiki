###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetWindowMinimumSize

Set the minimum size of a window's client area.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void SDL_SetWindowMinimumSize(SDL_Window * window,
                              int min_w, int min_h);
```

## Function Parameters

|                            |            |                                             |
| -------------------------- | ---------- | ------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to change.                       |
| int                        | **min_w**  | the minimum width of the window in pixels.  |
| int                        | **min_h**  | the minimum height of the window in pixels. |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetWindowMinimumSize](SDL_GetWindowMinimumSize)
- [SDL_SetWindowMaximumSize](SDL_SetWindowMaximumSize)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

