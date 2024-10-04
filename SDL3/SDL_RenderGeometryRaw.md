###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_RenderGeometryRaw

Render a list of triangles, optionally using a texture and indices into the vertex arrays Color and alpha modulation is done per vertex ([SDL_SetTextureColorMod](SDL_SetTextureColorMod) and [SDL_SetTextureAlphaMod](SDL_SetTextureAlphaMod) are ignored).

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
bool SDL_RenderGeometryRaw(SDL_Renderer *renderer,
                   SDL_Texture *texture,
                   const float *xy, int xy_stride,
                   const SDL_FColor *color, int color_stride,
                   const float *uv, int uv_stride,
                   int num_vertices,
                   const void *indices, int num_indices, int size_indices);
```

## Function Parameters

|                                  |                  |                                                                                                                       |
| -------------------------------- | ---------------- | --------------------------------------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) *   | **renderer**     | the rendering context.                                                                                                |
| [SDL_Texture](SDL_Texture) *     | **texture**      | (optional) The SDL texture to use.                                                                                    |
| const float *                    | **xy**           | vertex positions.                                                                                                     |
| int                              | **xy_stride**    | byte size to move from one element to the next element.                                                               |
| const [SDL_FColor](SDL_FColor) * | **color**        | vertex colors (as [SDL_FColor](SDL_FColor)).                                                                          |
| int                              | **color_stride** | byte size to move from one element to the next element.                                                               |
| const float *                    | **uv**           | vertex normalized texture coordinates.                                                                                |
| int                              | **uv_stride**    | byte size to move from one element to the next element.                                                               |
| int                              | **num_vertices** | number of vertices.                                                                                                   |
| const void *                     | **indices**      | (optional) An array of indices into the 'vertices' arrays, if NULL all vertices will be rendered in sequential order. |
| int                              | **num_indices**  | number of indices.                                                                                                    |
| int                              | **size_indices** | index size: 1 (byte), 2 (short), 4 (int).                                                                             |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Thread Safety

You may only call this function from the main thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_RenderGeometry](SDL_RenderGeometry)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

