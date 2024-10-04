###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetSurfaceBlendMode

Set the blend mode used for blit operations.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
int SDL_SetSurfaceBlendMode(SDL_Surface * surface,
                            SDL_BlendMode blendMode);
```

## Function Parameters

|                                |               |                                                              |
| ------------------------------ | ------------- | ------------------------------------------------------------ |
| [SDL_Surface](SDL_Surface) *   | **surface**   | the [SDL_Surface](SDL_Surface) structure to update.          |
| [SDL_BlendMode](SDL_BlendMode) | **blendMode** | the [SDL_BlendMode](SDL_BlendMode) to use for blit blending. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

To copy a surface to another surface (or texture) without blending with the
existing data, the blendmode of the SOURCE surface should be set to
[`SDL_BLENDMODE_NONE`](SDL_BLENDMODE_NONE).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetSurfaceBlendMode](SDL_GetSurfaceBlendMode)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

