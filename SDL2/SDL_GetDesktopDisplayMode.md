###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetDesktopDisplayMode

Get information about the desktop's display mode.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_GetDesktopDisplayMode(int displayIndex, SDL_DisplayMode * mode);
```

## Function Parameters

|                                      |                  |                                                                                          |
| ------------------------------------ | ---------------- | ---------------------------------------------------------------------------------------- |
| int                                  | **displayIndex** | the index of the display to query.                                                       |
| [SDL_DisplayMode](SDL_DisplayMode) * | **mode**         | an [SDL_DisplayMode](SDL_DisplayMode) structure filled in with the current display mode. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

There's a difference between this function and
[SDL_GetCurrentDisplayMode](SDL_GetCurrentDisplayMode)() when SDL runs
fullscreen and has changed the resolution. In that case this function will
return the previous native display mode, and not the current display mode.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetCurrentDisplayMode](SDL_GetCurrentDisplayMode)
- [SDL_GetDisplayMode](SDL_GetDisplayMode)
- [SDL_SetWindowDisplayMode](SDL_SetWindowDisplayMode)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

