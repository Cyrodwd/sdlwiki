# SDL_RenderGetClipRect

Get the clip rectangle for the current target.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
void SDL_RenderGetClipRect(SDL_Renderer * renderer,
                           SDL_Rect * rect);
```

## Function Parameters

|                                |              |                                                                                                                           |
| ------------------------------ | ------------ | ------------------------------------------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context from which clip rectangle should be queried.                                                        |
| [SDL_Rect](SDL_Rect) *         | **rect**     | an [SDL_Rect](SDL_Rect) structure filled in with the current clipping area or an empty rectangle if clipping is disabled. |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_RenderIsClipEnabled](SDL_RenderIsClipEnabled)
- [SDL_RenderSetClipRect](SDL_RenderSetClipRect)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

