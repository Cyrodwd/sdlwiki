# SDL_RenderTargetSupported

Determine whether a renderer supports the use of render targets.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
SDL_bool SDL_RenderTargetSupported(SDL_Renderer *renderer);
```

## Function Parameters

|                                |              |                                    |
| ------------------------------ | ------------ | ---------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the renderer that will be checked. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if supported or
[SDL_FALSE](SDL_FALSE) if not.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetRenderTarget](SDL_SetRenderTarget)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

