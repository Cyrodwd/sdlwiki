###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_FreeFormat

Free an [SDL_PixelFormat](SDL_PixelFormat) structure allocated by [SDL_AllocFormat](SDL_AllocFormat)().

## Header File

Defined in [SDL_pixels.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_pixels.h)

## Syntax

```c
void SDL_FreeFormat(SDL_PixelFormat *format);
```

## Function Parameters

|                                      |            |                                                           |
| ------------------------------------ | ---------- | --------------------------------------------------------- |
| [SDL_PixelFormat](SDL_PixelFormat) * | **format** | the [SDL_PixelFormat](SDL_PixelFormat) structure to free. |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_AllocFormat](SDL_AllocFormat)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

