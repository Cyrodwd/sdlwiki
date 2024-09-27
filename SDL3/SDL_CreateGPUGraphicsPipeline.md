###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_CreateGPUGraphicsPipeline

Creates a pipeline object to be used in a graphics workflow.

## Header File

Defined in [<SDL3/SDL_gpu.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gpu.h)

## Syntax

```c
SDL_GPUGraphicsPipeline* SDL_CreateGPUGraphicsPipeline(
    SDL_GPUDevice *device,
    const SDL_GPUGraphicsPipelineCreateInfo *createinfo);
```

## Function Parameters

|                                                                                |                |                                                                   |
| ------------------------------------------------------------------------------ | -------------- | ----------------------------------------------------------------- |
| [SDL_GPUDevice](SDL_GPUDevice) *                                               | **device**     | a GPU Context.                                                    |
| const [SDL_GPUGraphicsPipelineCreateInfo](SDL_GPUGraphicsPipelineCreateInfo) * | **createinfo** | a struct describing the state of the graphics pipeline to create. |

## Return Value

([SDL_GPUGraphicsPipeline](SDL_GPUGraphicsPipeline) *) Returns a graphics
pipeline object on success, or NULL on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_CreateGPUShader](SDL_CreateGPUShader)
- [SDL_BindGPUGraphicsPipeline](SDL_BindGPUGraphicsPipeline)
- [SDL_ReleaseGPUGraphicsPipeline](SDL_ReleaseGPUGraphicsPipeline)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGPU](CategoryGPU)

