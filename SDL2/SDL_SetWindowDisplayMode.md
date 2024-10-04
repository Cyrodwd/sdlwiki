###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetWindowDisplayMode

Set the display mode to use when a window is visible at fullscreen.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_SetWindowDisplayMode(SDL_Window * window,
                         const SDL_DisplayMode * mode);
```

## Function Parameters

|                                            |            |                                                                                                                                                                  |
| ------------------------------------------ | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) *                 | **window** | the window to affect.                                                                                                                                            |
| const [SDL_DisplayMode](SDL_DisplayMode) * | **mode**   | the [SDL_DisplayMode](SDL_DisplayMode) structure representing the mode to use, or NULL to use the window's dimensions and the desktop's format and refresh rate. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This only affects the display mode used when the window is fullscreen. To
change the window size when the window is not fullscreen, use
[SDL_SetWindowSize](SDL_SetWindowSize)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetWindowDisplayMode](SDL_GetWindowDisplayMode)
- [SDL_SetWindowFullscreen](SDL_SetWindowFullscreen)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

