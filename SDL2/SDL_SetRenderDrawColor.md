###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetRenderDrawColor

Set the color used for drawing operations (Rect, Line and Clear).

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_SetRenderDrawColor(SDL_Renderer * renderer,
                   Uint8 r, Uint8 g, Uint8 b,
                   Uint8 a);
```

## Function Parameters

|                                |              |                                                                                                                                                                                                                    |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.                                                                                                                                                                                             |
| Uint8                          | **r**        | the red value used to draw on the rendering target.                                                                                                                                                                |
| Uint8                          | **g**        | the green value used to draw on the rendering target.                                                                                                                                                              |
| Uint8                          | **b**        | the blue value used to draw on the rendering target.                                                                                                                                                               |
| Uint8                          | **a**        | the alpha value used to draw on the rendering target; usually [`SDL_ALPHA_OPAQUE`](SDL_ALPHA_OPAQUE) (255). Use [SDL_SetRenderDrawBlendMode](SDL_SetRenderDrawBlendMode) to specify how the alpha channel is used. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Set the color for drawing or filling rectangles, lines, and points, and for
[SDL_RenderClear](SDL_RenderClear)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetRenderDrawColor](SDL_GetRenderDrawColor)
- [SDL_RenderClear](SDL_RenderClear)
- [SDL_RenderDrawLine](SDL_RenderDrawLine)
- [SDL_RenderDrawLines](SDL_RenderDrawLines)
- [SDL_RenderDrawPoint](SDL_RenderDrawPoint)
- [SDL_RenderDrawPoints](SDL_RenderDrawPoints)
- [SDL_RenderDrawRect](SDL_RenderDrawRect)
- [SDL_RenderDrawRects](SDL_RenderDrawRects)
- [SDL_RenderFillRect](SDL_RenderFillRect)
- [SDL_RenderFillRects](SDL_RenderFillRects)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

