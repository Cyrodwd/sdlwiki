# SDL_GetRenderDrawColor

Get the color used for drawing operations (Rect, Line and Clear).

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_GetRenderDrawColor(SDL_Renderer * renderer,
                   Uint8 * r, Uint8 * g, Uint8 * b,
                   Uint8 * a);
```

## Function Parameters

|                                |              |                                                                                                                                      |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.                                                                                                               |
| Uint8 *                        | **r**        | a pointer filled in with the red value used to draw on the rendering target.                                                         |
| Uint8 *                        | **g**        | a pointer filled in with the green value used to draw on the rendering target.                                                       |
| Uint8 *                        | **b**        | a pointer filled in with the blue value used to draw on the rendering target.                                                        |
| Uint8 *                        | **a**        | a pointer filled in with the alpha value used to draw on the rendering target; usually [`SDL_ALPHA_OPAQUE`](SDL_ALPHA_OPAQUE) (255). |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetRenderDrawColor](SDL_SetRenderDrawColor)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

