# SDL_RenderSetVSync

Toggle VSync of the given renderer.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_RenderSetVSync(SDL_Renderer* renderer, int vsync);
```

## Function Parameters

|                                |              |                                                     |
| ------------------------------ | ------------ | --------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | The renderer to toggle.                             |
| int                            | **vsync**    | 1 for on, 0 for off. All other values are reserved. |

## Return Value

(int) Returns a 0 int on success, or non-zero on failure.

## Version

This function is available since SDL 2.0.18.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

