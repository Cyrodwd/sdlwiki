# SDL_RenderCopyEx

Copy a portion of the texture to the current rendering, with optional rotation and flipping.

## Header File

Defined in [SDL_render.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_render.h)

## Syntax

```c
int SDL_RenderCopyEx(SDL_Renderer * renderer,
                   SDL_Texture * texture,
                   const SDL_Rect * srcrect,
                   const SDL_Rect * dstrect,
                   const double angle,
                   const SDL_Point *center,
                   const SDL_RendererFlip flip);
```

## Function Parameters

|                                            |              |                                                                                                                                                          |
| ------------------------------------------ | ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) *             | **renderer** | the rendering context.                                                                                                                                   |
| [SDL_Texture](SDL_Texture) *               | **texture**  | the source texture.                                                                                                                                      |
| const [SDL_Rect](SDL_Rect) *               | **srcrect**  | the source [SDL_Rect](SDL_Rect) structure or NULL for the entire texture.                                                                                |
| const [SDL_Rect](SDL_Rect) *               | **dstrect**  | the destination [SDL_Rect](SDL_Rect) structure or NULL for the entire rendering target.                                                                  |
| const double                               | **angle**    | an angle in degrees that indicates the rotation that will be applied to dstrect, rotating it in a clockwise direction.                                   |
| const [SDL_Point](SDL_Point) *             | **center**   | a pointer to a point indicating the point around which dstrect will be rotated (if NULL, rotation will be done around `dstrect.w / 2`, `dstrect.h / 2`). |
| const [SDL_RendererFlip](SDL_RendererFlip) | **flip**     | a [SDL_RendererFlip](SDL_RendererFlip) value stating which flipping actions should be performed on the texture.                                          |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Copy a portion of the texture to the current rendering target, optionally
rotating it by angle around the given center and also flipping it
top-bottom and/or left-right.

The texture is blended with the destination based on its blend mode set
with [SDL_SetTextureBlendMode](SDL_SetTextureBlendMode)().

The texture color is affected based on its color modulation set by
[SDL_SetTextureColorMod](SDL_SetTextureColorMod)().

The texture alpha is affected based on its alpha modulation set by
[SDL_SetTextureAlphaMod](SDL_SetTextureAlphaMod)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_RenderCopy](SDL_RenderCopy)
- [SDL_SetTextureAlphaMod](SDL_SetTextureAlphaMod)
- [SDL_SetTextureBlendMode](SDL_SetTextureBlendMode)
- [SDL_SetTextureColorMod](SDL_SetTextureColorMod)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

