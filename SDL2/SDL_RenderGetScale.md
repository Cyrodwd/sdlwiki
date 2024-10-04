###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_RenderGetScale

Get the drawing scale for the current target.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
void SDL_RenderGetScale(SDL_Renderer * renderer,
                   float *scaleX, float *scaleY);
```

## Function Parameters

|                                |              |                                                          |
| ------------------------------ | ------------ | -------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the renderer from which drawing scale should be queried. |
| float *                        | **scaleX**   | a pointer filled in with the horizontal scaling factor.  |
| float *                        | **scaleY**   | a pointer filled in with the vertical scaling factor.    |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_RenderSetScale](SDL_RenderSetScale)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

