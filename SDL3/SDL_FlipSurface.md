###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_FlipSurface

Flip a surface vertically or horizontally.

## Header File

Defined in [<SDL3/SDL_surface.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_surface.h)

## Syntax

```c
bool SDL_FlipSurface(SDL_Surface *surface, SDL_FlipMode flip);
```

## Function Parameters

|                              |             |                        |
| ---------------------------- | ----------- | ---------------------- |
| [SDL_Surface](SDL_Surface) * | **surface** | the surface to flip.   |
| [SDL_FlipMode](SDL_FlipMode) | **flip**    | the direction to flip. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

