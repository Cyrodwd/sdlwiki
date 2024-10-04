###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_RenderWindowToLogical

Get logical coordinates of point in renderer when given real coordinates of point in window.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
void SDL_RenderWindowToLogical(SDL_Renderer * renderer, 
                                int windowX, int windowY, 
                                float *logicalX, float *logicalY);
```

## Function Parameters

|                                |              |                                                                       |
| ------------------------------ | ------------ | --------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the renderer from which the logical coordinates should be calculated. |
| int                            | **windowX**  | the real X coordinate in the window.                                  |
| int                            | **windowY**  | the real Y coordinate in the window.                                  |
| float *                        | **logicalX** | the pointer filled with the logical x coordinate.                     |
| float *                        | **logicalY** | the pointer filled with the logical y coordinate.                     |

## Remarks

Logical coordinates will differ from real coordinates when render is scaled
and logical renderer size set

## Version

This function is available since SDL 2.0.18.

## See Also

- [SDL_RenderGetScale](SDL_RenderGetScale)
- [SDL_RenderSetScale](SDL_RenderSetScale)
- [SDL_RenderGetLogicalSize](SDL_RenderGetLogicalSize)
- [SDL_RenderSetLogicalSize](SDL_RenderSetLogicalSize)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

