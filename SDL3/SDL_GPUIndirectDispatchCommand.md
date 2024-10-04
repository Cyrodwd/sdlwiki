###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GPUIndirectDispatchCommand

A structure specifying the parameters of an indexed dispatch command.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
typedef struct SDL_GPUIndirectDispatchCommand
{
    Uint32 groupcount_x;  /**< The number of local workgroups to dispatch in the X dimension. */
    Uint32 groupcount_y;  /**< The number of local workgroups to dispatch in the Y dimension. */
    Uint32 groupcount_z;  /**< The number of local workgroups to dispatch in the Z dimension. */
} SDL_GPUIndirectDispatchCommand;
```

## Version

This struct is available since SDL 3.0.0

## See Also

- [SDL_DispatchGPUComputeIndirect](SDL_DispatchGPUComputeIndirect)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIStruct](CategoryAPIStruct), [CategoryGPU](CategoryGPU)

