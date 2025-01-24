# SDL_LockSurface

Set up a surface for directly accessing the pixels.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
int SDL_LockSurface(SDL_Surface * surface);
```

## Function Parameters

|                              |             |                                                        |
| ---------------------------- | ----------- | ------------------------------------------------------ |
| [SDL_Surface](SDL_Surface) * | **surface** | the [SDL_Surface](SDL_Surface) structure to be locked. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Between calls to [SDL_LockSurface](SDL_LockSurface)() /
[SDL_UnlockSurface](SDL_UnlockSurface)(), you can write to and read from
`surface->pixels`, using the pixel format stored in `surface->format`. Once
you are done accessing the surface, you should use
[SDL_UnlockSurface](SDL_UnlockSurface)() to release it.

Not all surfaces require locking. If `SDL_MUSTLOCK(surface)` evaluates to
0, then you can read and write to the surface at any time, and the pixel
format of the surface will not change.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_MUSTLOCK](SDL_MUSTLOCK)
- [SDL_UnlockSurface](SDL_UnlockSurface)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

