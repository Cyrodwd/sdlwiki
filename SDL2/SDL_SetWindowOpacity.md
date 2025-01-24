# SDL_SetWindowOpacity

Set the opacity for a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_SetWindowOpacity(SDL_Window * window, float opacity);
```

## Function Parameters

|                            |             |                                                        |
| -------------------------- | ----------- | ------------------------------------------------------ |
| [SDL_Window](SDL_Window) * | **window**  | the window which will be made transparent or opaque.   |
| float                      | **opacity** | the opacity value (0.0f - transparent, 1.0f - opaque). |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The parameter `opacity` will be clamped internally between 0.0f
(transparent) and 1.0f (opaque).

This function also returns -1 if setting the opacity isn't supported.

## Version

This function is available since SDL 2.0.5.

## See Also

- [SDL_GetWindowOpacity](SDL_GetWindowOpacity)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

