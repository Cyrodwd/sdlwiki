###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_GetRenderDrawColorFloat

Get the color used for drawing operations (Rect, Line and Clear).

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
bool SDL_GetRenderDrawColorFloat(SDL_Renderer *renderer, float *r, float *g, float *b, float *a);
```

## Function Parameters

|                                |              |                                                                                |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------ |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.                                                         |
| float *                        | **r**        | a pointer filled in with the red value used to draw on the rendering target.   |
| float *                        | **g**        | a pointer filled in with the green value used to draw on the rendering target. |
| float *                        | **b**        | a pointer filled in with the blue value used to draw on the rendering target.  |
| float *                        | **a**        | a pointer filled in with the alpha value used to draw on the rendering target. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Thread Safety

You may only call this function from the main thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_SetRenderDrawColorFloat](SDL_SetRenderDrawColorFloat)
- [SDL_GetRenderDrawColor](SDL_GetRenderDrawColor)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

