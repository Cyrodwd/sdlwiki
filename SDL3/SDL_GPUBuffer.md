# SDL_GPUBuffer

An opaque handle representing a buffer.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
typedef struct SDL_GPUBuffer SDL_GPUBuffer;
```

## Remarks

Used for vertices, indices, indirect draw commands, and general compute
data.

## Version

This struct is available since SDL 3.2.0.

## See Also

- [SDL_CreateGPUBuffer](SDL_CreateGPUBuffer)
- [SDL_UploadToGPUBuffer](SDL_UploadToGPUBuffer)
- [SDL_DownloadFromGPUBuffer](SDL_DownloadFromGPUBuffer)
- [SDL_CopyGPUBufferToBuffer](SDL_CopyGPUBufferToBuffer)
- [SDL_BindGPUVertexBuffers](SDL_BindGPUVertexBuffers)
- [SDL_BindGPUIndexBuffer](SDL_BindGPUIndexBuffer)
- [SDL_BindGPUVertexStorageBuffers](SDL_BindGPUVertexStorageBuffers)
- [SDL_BindGPUFragmentStorageBuffers](SDL_BindGPUFragmentStorageBuffers)
- [SDL_DrawGPUPrimitivesIndirect](SDL_DrawGPUPrimitivesIndirect)
- [SDL_DrawGPUIndexedPrimitivesIndirect](SDL_DrawGPUIndexedPrimitivesIndirect)
- [SDL_BindGPUComputeStorageBuffers](SDL_BindGPUComputeStorageBuffers)
- [SDL_DispatchGPUComputeIndirect](SDL_DispatchGPUComputeIndirect)
- [SDL_ReleaseGPUBuffer](SDL_ReleaseGPUBuffer)

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryGPU](CategoryGPU)

