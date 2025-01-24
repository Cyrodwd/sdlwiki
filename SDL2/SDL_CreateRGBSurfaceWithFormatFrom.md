# SDL_CreateRGBSurfaceWithFormatFrom

Allocate a new RGB surface with with a specific pixel format and existing pixel data.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
SDL_Surface* SDL_CreateRGBSurfaceWithFormatFrom
    (void *pixels, int width, int height, int depth, int pitch, Uint32 format);
```

## Function Parameters

|                  |            |                                                                                    |
| ---------------- | ---------- | ---------------------------------------------------------------------------------- |
| void *           | **pixels** | a pointer to existing pixel data.                                                  |
| int              | **width**  | the width of the surface.                                                          |
| int              | **height** | the height of the surface.                                                         |
| int              | **depth**  | the depth of the surface in bits.                                                  |
| int              | **pitch**  | the pitch of the surface in bytes.                                                 |
| [Uint32](Uint32) | **format** | the [SDL_PixelFormatEnum](SDL_PixelFormatEnum) for the new surface's pixel format. |

## Return Value

([SDL_Surface](SDL_Surface) *) Returns the new [SDL_Surface](SDL_Surface)
structure that is created or NULL if it fails; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function operates mostly like
[SDL_CreateRGBSurfaceFrom](SDL_CreateRGBSurfaceFrom)(), except instead of
providing pixel color masks, you provide it with a predefined format from
[SDL_PixelFormatEnum](SDL_PixelFormatEnum).

No copy is made of the pixel data. Pixel data is not managed automatically;
you must free the surface before you free the pixel data.

## Version

This function is available since SDL 2.0.5.

## See Also

- [SDL_CreateRGBSurfaceFrom](SDL_CreateRGBSurfaceFrom)
- [SDL_CreateRGBSurfaceWithFormat](SDL_CreateRGBSurfaceWithFormat)
- [SDL_FreeSurface](SDL_FreeSurface)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

