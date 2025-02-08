# SDL_GetWindowDisplayMode

Query the display mode to use when a window is visible at fullscreen.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_GetWindowDisplayMode(SDL_Window * window,
                             SDL_DisplayMode * mode);
```

## Function Parameters

|                                      |            |                                                                                             |
| ------------------------------------ | ---------- | ------------------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) *           | **window** | the window to query.                                                                        |
| [SDL_DisplayMode](SDL_DisplayMode) * | **mode**   | an [SDL_DisplayMode](SDL_DisplayMode) structure filled in with the fullscreen display mode. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetWindowDisplayMode](SDL_SetWindowDisplayMode)
- [SDL_SetWindowFullscreen](SDL_SetWindowFullscreen)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

