###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetWindowResizable

Set the user-resizable state of a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void SDL_SetWindowResizable(SDL_Window * window,
                            SDL_bool resizable);
```

## Function Parameters

|                            |               |                                                                             |
| -------------------------- | ------------- | --------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window**    | the window of which to change the resizable state.                          |
| [SDL_bool](SDL_bool)       | **resizable** | [SDL_TRUE](SDL_TRUE) to allow resizing, [SDL_FALSE](SDL_FALSE) to disallow. |

## Remarks

This will add or remove the window's
[`SDL_WINDOW_RESIZABLE`](SDL_WINDOW_RESIZABLE) flag and allow/disallow user
resizing of the window. This is a no-op if the window's resizable state
already matches the requested state.

You can't change the resizable state of a fullscreen window.

## Version

This function is available since SDL 2.0.5.

## See Also

- [SDL_GetWindowFlags](SDL_GetWindowFlags)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

