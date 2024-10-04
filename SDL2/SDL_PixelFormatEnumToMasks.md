###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_PixelFormatEnumToMasks

Convert one of the enumerated pixel formats to a bpp value and RGBA masks.

## Header File

Defined in [SDL_pixels.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_pixels.h)

## Syntax

```c
SDL_bool SDL_PixelFormatEnumToMasks(Uint32 format,
                                    int *bpp,
                                    Uint32 * Rmask,
                                    Uint32 * Gmask,
                                    Uint32 * Bmask,
                                    Uint32 * Amask);
```

## Function Parameters

|          |            |                                                               |
| -------- | ---------- | ------------------------------------------------------------- |
| Uint32   | **format** | one of the [SDL_PixelFormatEnum](SDL_PixelFormatEnum) values. |
| int *    | **bpp**    | a bits per pixel value; usually 15, 16, or 32.                |
| Uint32 * | **Rmask**  | a pointer filled in with the red mask for the format.         |
| Uint32 * | **Gmask**  | a pointer filled in with the green mask for the format.       |
| Uint32 * | **Bmask**  | a pointer filled in with the blue mask for the format.        |
| Uint32 * | **Amask**  | a pointer filled in with the alpha mask for the format.       |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) on success or
[SDL_FALSE](SDL_FALSE) if the conversion wasn't possible; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_MasksToPixelFormatEnum](SDL_MasksToPixelFormatEnum)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

