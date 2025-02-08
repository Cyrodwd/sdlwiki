# SDL_MasksToPixelFormatEnum

Convert a bpp value and RGBA masks to an enumerated pixel format.

## Header File

Defined in [SDL_pixels.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_pixels.h)

## Syntax

```c
Uint32 SDL_MasksToPixelFormatEnum(int bpp,
                                  Uint32 Rmask,
                                  Uint32 Gmask,
                                  Uint32 Bmask,
                                  Uint32 Amask);
```

## Function Parameters

|                  |           |                                                |
| ---------------- | --------- | ---------------------------------------------- |
| int              | **bpp**   | a bits per pixel value; usually 15, 16, or 32. |
| [Uint32](Uint32) | **Rmask** | the red mask for the format.                   |
| [Uint32](Uint32) | **Gmask** | the green mask for the format.                 |
| [Uint32](Uint32) | **Bmask** | the blue mask for the format.                  |
| [Uint32](Uint32) | **Amask** | the alpha mask for the format.                 |

## Return Value

([Uint32](Uint32)) Returns one of the
[SDL_PixelFormatEnum](SDL_PixelFormatEnum) values.

## Remarks

This will return [`SDL_PIXELFORMAT_UNKNOWN`](SDL_PIXELFORMAT_UNKNOWN) if
the conversion wasn't possible.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_PixelFormatEnumToMasks](SDL_PixelFormatEnumToMasks)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

