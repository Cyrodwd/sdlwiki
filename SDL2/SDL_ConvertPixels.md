###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_ConvertPixels

Copy a block of pixels of one format to another format.

## Header File

Defined in [SDL_surface.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_surface.h)

## Syntax

```c
int SDL_ConvertPixels(int width, int height,
                      Uint32 src_format,
                      const void * src, int src_pitch,
                      Uint32 dst_format,
                      void * dst, int dst_pitch);
```

## Function Parameters

|              |                |                                                                                 |
| ------------ | -------------- | ------------------------------------------------------------------------------- |
| int          | **width**      | the width of the block to copy, in pixels.                                      |
| int          | **height**     | the height of the block to copy, in pixels.                                     |
| Uint32       | **src_format** | an [SDL_PixelFormatEnum](SDL_PixelFormatEnum) value of the `src` pixels format. |
| const void * | **src**        | a pointer to the source pixels.                                                 |
| int          | **src_pitch**  | the pitch of the source pixels, in bytes.                                       |
| Uint32       | **dst_format** | an [SDL_PixelFormatEnum](SDL_PixelFormatEnum) value of the `dst` pixels format. |
| void *       | **dst**        | a pointer to be filled in with new pixel data.                                  |
| int          | **dst_pitch**  | the pitch of the destination pixels, in bytes.                                  |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

