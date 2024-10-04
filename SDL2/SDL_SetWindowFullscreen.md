###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetWindowFullscreen

Set a window's fullscreen state.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_SetWindowFullscreen(SDL_Window * window,
                            Uint32 flags);
```

## Function Parameters

|                            |            |                                                                                                                          |
| -------------------------- | ---------- | ------------------------------------------------------------------------------------------------------------------------ |
| [SDL_Window](SDL_Window) * | **window** | the window to change.                                                                                                    |
| Uint32                     | **flags**  | [`SDL_WINDOW_FULLSCREEN`](SDL_WINDOW_FULLSCREEN), [`SDL_WINDOW_FULLSCREEN_DESKTOP`](SDL_WINDOW_FULLSCREEN_DESKTOP) or 0. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

`flags` may be [`SDL_WINDOW_FULLSCREEN`](SDL_WINDOW_FULLSCREEN), for "real"
fullscreen with a videomode change;
[`SDL_WINDOW_FULLSCREEN_DESKTOP`](SDL_WINDOW_FULLSCREEN_DESKTOP) for "fake"
fullscreen that takes the size of the desktop; and 0 for windowed mode.

Note that for some renderers, this function may trigger an
[SDL_RENDER_TARGETS_RESET](SDL_RENDER_TARGETS_RESET) event. Your
application should be prepared to handle this event by reuploading
textures!

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetWindowDisplayMode](SDL_GetWindowDisplayMode)
- [SDL_SetWindowDisplayMode](SDL_SetWindowDisplayMode)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

