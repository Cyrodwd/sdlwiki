# SDL_GetWindowGrab

Get a window's input grab mode.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
SDL_bool SDL_GetWindowGrab(SDL_Window * window);
```

## Function Parameters

|                            |            |                      |
| -------------------------- | ---------- | -------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to query. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if input is grabbed,
[SDL_FALSE](SDL_FALSE) otherwise.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetWindowGrab](SDL_SetWindowGrab)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

