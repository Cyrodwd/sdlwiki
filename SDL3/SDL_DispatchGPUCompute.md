###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_DispatchGPUCompute

Dispatches compute work.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
void SDL_DispatchGPUCompute(
    SDL_GPUComputePass *compute_pass,
    Uint32 groupcount_x,
    Uint32 groupcount_y,
    Uint32 groupcount_z);
```

## Function Parameters

|                                            |                  |                                                            |
| ------------------------------------------ | ---------------- | ---------------------------------------------------------- |
| [SDL_GPUComputePass](SDL_GPUComputePass) * | **compute_pass** | a compute pass handle.                                     |
| Uint32                                     | **groupcount_x** | number of local workgroups to dispatch in the X dimension. |
| Uint32                                     | **groupcount_y** | number of local workgroups to dispatch in the Y dimension. |
| Uint32                                     | **groupcount_z** | number of local workgroups to dispatch in the Z dimension. |

## Remarks

You must not call this function before binding a compute pipeline.

A VERY IMPORTANT NOTE If you dispatch multiple times in a compute pass, and
the dispatches write to the same resource region as each other, there is no
guarantee of which order the writes will occur. If the write order matters,
you MUST end the compute pass and begin another one.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGPU](CategoryGPU)

