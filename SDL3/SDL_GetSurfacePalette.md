# SDL_GetSurfacePalette

Get the palette used by a surface.

## Header File

Defined in [<SDL3/SDL_surface.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_surface.h)

## Syntax

```c
SDL_Palette * SDL_GetSurfacePalette(SDL_Surface *surface);
```

## Function Parameters

|                              |             |                                                    |
| ---------------------------- | ----------- | -------------------------------------------------- |
| [SDL_Surface](SDL_Surface) * | **surface** | the [SDL_Surface](SDL_Surface) structure to query. |

## Return Value

([SDL_Palette](SDL_Palette) *) Returns a pointer to the palette used by the
surface, or NULL if there is no palette used.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_SetSurfacePalette](SDL_SetSurfacePalette)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

