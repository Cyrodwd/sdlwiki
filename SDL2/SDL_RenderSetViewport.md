###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_RenderSetViewport

Set the drawing area for rendering on the current target.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_RenderSetViewport(SDL_Renderer * renderer,
                      const SDL_Rect * rect);
```

## Function Parameters

|                                |              |                                                                                                                     |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.                                                                                              |
| const [SDL_Rect](SDL_Rect) *   | **rect**     | the [SDL_Rect](SDL_Rect) structure representing the drawing area, or NULL to set the viewport to the entire target. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

When the window is resized, the viewport is reset to fill the entire new
window size.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_RenderGetViewport](SDL_RenderGetViewport)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

