###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetRendererOutputSize

Get the output size in pixels of a rendering context.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_GetRendererOutputSize(SDL_Renderer * renderer,
                              int *w, int *h);
```

## Function Parameters

|                                |              |                                |
| ------------------------------ | ------------ | ------------------------------ |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.         |
| int *                          | **w**        | an int filled with the width.  |
| int *                          | **h**        | an int filled with the height. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Due to high-dpi displays, you might end up with a rendering context that
has more pixels than the window that contains it, so use this instead of
[SDL_GetWindowSize](SDL_GetWindowSize)() to decide how much drawing area
you have.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetRenderer](SDL_GetRenderer)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

