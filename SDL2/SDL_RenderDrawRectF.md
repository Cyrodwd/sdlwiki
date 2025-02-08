# SDL_RenderDrawRectF

Draw a rectangle on the current rendering target at subpixel precision.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_RenderDrawRectF(SDL_Renderer * renderer,
                        const SDL_FRect * rect);
```

## Function Parameters

|                                |              |                                                                                         |
| ------------------------------ | ------------ | --------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | The renderer which should draw a rectangle.                                             |
| const [SDL_FRect](SDL_FRect) * | **rect**     | A pointer to the destination rectangle, or NULL to outline the entire rendering target. |

## Return Value

(int) Return 0 on success, or -1 on error.

## Version

This function is available since SDL 2.0.10.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

