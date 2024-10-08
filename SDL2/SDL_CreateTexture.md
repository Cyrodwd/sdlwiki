###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_CreateTexture

Create a texture for a rendering context.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
SDL_Texture * SDL_CreateTexture(SDL_Renderer * renderer,
                                Uint32 format,
                                int access, int w,
                                int h);
```

## Function Parameters

|                                |              |                                                                             |
| ------------------------------ | ------------ | --------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.                                                      |
| Uint32                         | **format**   | one of the enumerated values in [SDL_PixelFormatEnum](SDL_PixelFormatEnum). |
| int                            | **access**   | one of the enumerated values in [SDL_TextureAccess](SDL_TextureAccess).     |
| int                            | **w**        | the width of the texture in pixels.                                         |
| int                            | **h**        | the height of the texture in pixels.                                        |

## Return Value

([SDL_Texture](SDL_Texture) *) Returns a pointer to the created texture or
NULL if no rendering context was active, the format was unsupported, or the
width or height were out of range; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

You can set the texture scaling method by setting
[`SDL_HINT_RENDER_SCALE_QUALITY`](SDL_HINT_RENDER_SCALE_QUALITY) before
creating the texture.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateTextureFromSurface](SDL_CreateTextureFromSurface)
- [SDL_DestroyTexture](SDL_DestroyTexture)
- [SDL_QueryTexture](SDL_QueryTexture)
- [SDL_UpdateTexture](SDL_UpdateTexture)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

