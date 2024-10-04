###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_SetGPUBufferName

Sets an arbitrary string constant to label a buffer.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
void SDL_SetGPUBufferName(
    SDL_GPUDevice *device,
    SDL_GPUBuffer *buffer,
    const char *text);
```

## Function Parameters

|                                  |            |                                                            |
| -------------------------------- | ---------- | ---------------------------------------------------------- |
| [SDL_GPUDevice](SDL_GPUDevice) * | **device** | a GPU Context.                                             |
| [SDL_GPUBuffer](SDL_GPUBuffer) * | **buffer** | a buffer to attach the name to.                            |
| const char *                     | **text**   | a UTF-8 string constant to mark as the name of the buffer. |

## Remarks

Useful for debugging.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGPU](CategoryGPU)

