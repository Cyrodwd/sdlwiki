# SDL_GetRGBA

Get RGBA values from a pixel in the specified format.

## Header File

Defined in [SDL_pixels.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_pixels.h)

## Syntax

```c
void SDL_GetRGBA(Uint32 pixel,
                 const SDL_PixelFormat * format,
                 Uint8 * r, Uint8 * g, Uint8 * b,
                 Uint8 * a);
```

## Function Parameters

|                                            |            |                                                                                     |
| ------------------------------------------ | ---------- | ----------------------------------------------------------------------------------- |
| [Uint32](Uint32)                           | **pixel**  | a pixel value.                                                                      |
| const [SDL_PixelFormat](SDL_PixelFormat) * | **format** | an [SDL_PixelFormat](SDL_PixelFormat) structure describing the format of the pixel. |
| Uint8 *                                    | **r**      | a pointer filled in with the red component.                                         |
| Uint8 *                                    | **g**      | a pointer filled in with the green component.                                       |
| Uint8 *                                    | **b**      | a pointer filled in with the blue component.                                        |
| Uint8 *                                    | **a**      | a pointer filled in with the alpha component.                                       |

## Remarks

This function uses the entire 8-bit [0..255] range when converting color
components from pixel formats with less than 8-bits per RGB component
(e.g., a completely white pixel in 16-bit RGB565 format would return [0xff,
0xff, 0xff] not [0xf8, 0xfc, 0xf8]).

If the surface has no alpha component, the alpha will be returned as 0xff
(100% opaque).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetRGB](SDL_GetRGB)
- [SDL_MapRGB](SDL_MapRGB)
- [SDL_MapRGBA](SDL_MapRGBA)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

