# SDL_FreeSurface

Free an RGB surface.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
void SDL_FreeSurface(SDL_Surface * surface);
```

## Function Parameters

|                              |             |                                         |
| ---------------------------- | ----------- | --------------------------------------- |
| [SDL_Surface](SDL_Surface) * | **surface** | the [SDL_Surface](SDL_Surface) to free. |

## Remarks

It is safe to pass NULL to this function.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateRGBSurface](SDL_CreateRGBSurface)
- [SDL_CreateRGBSurfaceFrom](SDL_CreateRGBSurfaceFrom)
- [SDL_LoadBMP](SDL_LoadBMP)
- [SDL_LoadBMP_RW](SDL_LoadBMP_RW)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

