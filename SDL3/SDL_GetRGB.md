###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetRGB

Get RGB values from a pixel in the specified format.

## Header File

Defined in [<SDL3/SDL_pixels.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_pixels.h)

## Syntax

```c
void SDL_GetRGB(Uint32 pixel, const SDL_PixelFormatDetails *format, const SDL_Palette *palette, Uint8 *r, Uint8 *g, Uint8 *b);
```

## Function Parameters

|                                                          |             |                                                                                            |
| -------------------------------------------------------- | ----------- | ------------------------------------------------------------------------------------------ |
| Uint32                                                   | **pixel**   | a pixel value.                                                                             |
| const [SDL_PixelFormatDetails](SDL_PixelFormatDetails) * | **format**  | a pointer to [SDL_PixelFormatDetails](SDL_PixelFormatDetails) describing the pixel format. |
| const [SDL_Palette](SDL_Palette) *                       | **palette** | an optional palette for indexed formats, may be NULL.                                      |
| Uint8 *                                                  | **r**       | a pointer filled in with the red component, may be NULL.                                   |
| Uint8 *                                                  | **g**       | a pointer filled in with the green component, may be NULL.                                 |
| Uint8 *                                                  | **b**       | a pointer filled in with the blue component, may be NULL.                                  |

## Remarks

This function uses the entire 8-bit [0..255] range when converting color
components from pixel formats with less than 8-bits per RGB component
(e.g., a completely white pixel in 16-bit RGB565 format would return [0xff,
0xff, 0xff] not [0xf8, 0xfc, 0xf8]).

## Thread Safety

It is safe to call this function from any thread, as long as the palette is
not modified.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetPixelFormatDetails](SDL_GetPixelFormatDetails)
- [SDL_GetRGBA](SDL_GetRGBA)
- [SDL_MapRGB](SDL_MapRGB)
- [SDL_MapRGBA](SDL_MapRGBA)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

