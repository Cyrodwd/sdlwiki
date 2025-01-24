# SDL_RenderDrawRectsF

Draw some number of rectangles on the current rendering target at subpixel precision.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_RenderDrawRectsF(SDL_Renderer * renderer,
                         const SDL_FRect * rects,
                         int count);
```

## Function Parameters

|                                |              |                                                     |
| ------------------------------ | ------------ | --------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | The renderer which should draw multiple rectangles. |
| const [SDL_FRect](SDL_FRect) * | **rects**    | A pointer to an array of destination rectangles.    |
| int                            | **count**    | The number of rectangles.                           |

## Return Value

(int) Return 0 on success, or -1 on error.

## Version

This function is available since SDL 2.0.10.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

