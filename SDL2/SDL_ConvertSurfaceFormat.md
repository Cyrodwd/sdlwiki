###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_ConvertSurfaceFormat

Copy an existing surface to a new surface of the specified format enum.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
SDL_Surface* SDL_ConvertSurfaceFormat
    (SDL_Surface * src, Uint32 pixel_format, Uint32 flags);
```

## Function Parameters

|                              |                  |                                                                                       |
| ---------------------------- | ---------------- | ------------------------------------------------------------------------------------- |
| [SDL_Surface](SDL_Surface) * | **src**          | the existing [SDL_Surface](SDL_Surface) structure to convert.                         |
| Uint32                       | **pixel_format** | the [SDL_PixelFormatEnum](SDL_PixelFormatEnum) that the new surface is optimized for. |
| Uint32                       | **flags**        | the flags are unused and should be set to 0; this is a leftover from SDL 1.2's API.   |

## Return Value

([SDL_Surface](SDL_Surface) *) Returns the new [SDL_Surface](SDL_Surface)
structure that is created or NULL if it fails; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function operates just like
[SDL_ConvertSurface](SDL_ConvertSurface)(), but accepts an
[SDL_PixelFormatEnum](SDL_PixelFormatEnum) value instead of an
[SDL_PixelFormat](SDL_PixelFormat) structure. As such, it might be easier
to call but it doesn't have access to palette information for the
destination surface, in case that would be important.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_AllocFormat](SDL_AllocFormat)
- [SDL_ConvertSurface](SDL_ConvertSurface)
- [SDL_CreateRGBSurface](SDL_CreateRGBSurface)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

