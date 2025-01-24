# SDL_RenderCopy

Copy a portion of the texture to the current rendering target.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_RenderCopy(SDL_Renderer * renderer,
                   SDL_Texture * texture,
                   const SDL_Rect * srcrect,
                   const SDL_Rect * dstrect);
```

## Function Parameters

|                                |              |                                                                                                                                                    |
| ------------------------------ | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context.                                                                                                                             |
| [SDL_Texture](SDL_Texture) *   | **texture**  | the source texture.                                                                                                                                |
| const [SDL_Rect](SDL_Rect) *   | **srcrect**  | the source [SDL_Rect](SDL_Rect) structure or NULL for the entire texture.                                                                          |
| const [SDL_Rect](SDL_Rect) *   | **dstrect**  | the destination [SDL_Rect](SDL_Rect) structure or NULL for the entire rendering target; the texture will be stretched to fill the given rectangle. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The texture is blended with the destination based on its blend mode set
with [SDL_SetTextureBlendMode](SDL_SetTextureBlendMode)().

The texture color is affected based on its color modulation set by
[SDL_SetTextureColorMod](SDL_SetTextureColorMod)().

The texture alpha is affected based on its alpha modulation set by
[SDL_SetTextureAlphaMod](SDL_SetTextureAlphaMod)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_RenderCopyEx](SDL_RenderCopyEx)
- [SDL_SetTextureAlphaMod](SDL_SetTextureAlphaMod)
- [SDL_SetTextureBlendMode](SDL_SetTextureBlendMode)
- [SDL_SetTextureColorMod](SDL_SetTextureColorMod)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

