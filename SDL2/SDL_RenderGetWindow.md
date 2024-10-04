###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_RenderGetWindow

Get the window associated with a renderer.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
SDL_Window * SDL_RenderGetWindow(SDL_Renderer *renderer);
```

## Function Parameters

|                                |              |                        |
| ------------------------------ | ------------ | ---------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the renderer to query. |

## Return Value

([SDL_Window](SDL_Window) *) Returns the window on success or NULL on
failure; call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.22.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

