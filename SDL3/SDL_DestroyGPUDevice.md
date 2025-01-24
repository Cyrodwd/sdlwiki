# SDL_DestroyGPUDevice

Destroys a GPU context previously returned by [SDL_CreateGPUDevice](SDL_CreateGPUDevice).

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
void SDL_DestroyGPUDevice(SDL_GPUDevice *device);
```

## Function Parameters

|                                  |            |                           |
| -------------------------------- | ---------- | ------------------------- |
| [SDL_GPUDevice](SDL_GPUDevice) * | **device** | a GPU Context to destroy. |

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_CreateGPUDevice](SDL_CreateGPUDevice)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGPU](CategoryGPU)

