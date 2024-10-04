###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_PremultiplyAlpha

Premultiply the alpha on a block of pixels.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
int SDL_PremultiplyAlpha(int width, int height,
                         Uint32 src_format,
                         const void * src, int src_pitch,
                         Uint32 dst_format,
                         void * dst, int dst_pitch);
```

## Function Parameters

|              |                |                                                                                 |
| ------------ | -------------- | ------------------------------------------------------------------------------- |
| int          | **width**      | the width of the block to convert, in pixels.                                   |
| int          | **height**     | the height of the block to convert, in pixels.                                  |
| Uint32       | **src_format** | an [SDL_PixelFormatEnum](SDL_PixelFormatEnum) value of the `src` pixels format. |
| const void * | **src**        | a pointer to the source pixels.                                                 |
| int          | **src_pitch**  | the pitch of the source pixels, in bytes.                                       |
| Uint32       | **dst_format** | an [SDL_PixelFormatEnum](SDL_PixelFormatEnum) value of the `dst` pixels format. |
| void *       | **dst**        | a pointer to be filled in with premultiplied pixel data.                        |
| int          | **dst_pitch**  | the pitch of the destination pixels, in bytes.                                  |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This is safe to use with src == dst, but not for other overlapping areas.

This function is currently only implemented for
[SDL_PIXELFORMAT_ARGB8888](SDL_PIXELFORMAT_ARGB8888).

## Version

This function is available since SDL 2.0.18.

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

