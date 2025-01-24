# SDL_UpdateNVTexture

Update a rectangle within a planar NV12 or NV21 texture with new pixels.

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
bool SDL_UpdateNVTexture(SDL_Texture *texture,
                     const SDL_Rect *rect,
                     const Uint8 *Yplane, int Ypitch,
                     const Uint8 *UVplane, int UVpitch);
```

## Function Parameters

|                              |             |                                                                                       |
| ---------------------------- | ----------- | ------------------------------------------------------------------------------------- |
| [SDL_Texture](SDL_Texture) * | **texture** | the texture to update.                                                                |
| const [SDL_Rect](SDL_Rect) * | **rect**    | a pointer to the rectangle of pixels to update, or NULL to update the entire texture. |
| const Uint8 *                | **Yplane**  | the raw pixel data for the Y plane.                                                   |
| int                          | **Ypitch**  | the number of bytes between rows of pixel data for the Y plane.                       |
| const Uint8 *                | **UVplane** | the raw pixel data for the UV plane.                                                  |
| int                          | **UVpitch** | the number of bytes between rows of pixel data for the UV plane.                      |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

You can use [SDL_UpdateTexture](SDL_UpdateTexture)() as long as your pixel
data is a contiguous block of NV12/21 planes in the proper order, but this
function is available if your pixel data is not contiguous.

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_UpdateTexture](SDL_UpdateTexture)
- [SDL_UpdateYUVTexture](SDL_UpdateYUVTexture)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

