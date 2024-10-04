###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetRenderMetalLayer

Get the CAMetalLayer associated with the given Metal renderer.

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
void * SDL_GetRenderMetalLayer(SDL_Renderer *renderer);
```

## Function Parameters

|                                |              |                        |
| ------------------------------ | ------------ | ---------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the renderer to query. |

## Return Value

(void *) Returns a `CAMetalLayer *` on success, or NULL if the renderer
isn't a Metal renderer.

## Remarks

This function returns `void *`, so SDL doesn't have to include Metal's
headers, but it can be safely cast to a `CAMetalLayer *`.

## Thread Safety

You may only call this function from the main thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetRenderMetalCommandEncoder](SDL_GetRenderMetalCommandEncoder)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

