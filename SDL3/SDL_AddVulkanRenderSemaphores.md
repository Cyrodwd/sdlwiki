###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_AddVulkanRenderSemaphores

Add a set of synchronization semaphores for the current frame.

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
bool SDL_AddVulkanRenderSemaphores(SDL_Renderer *renderer, Uint32 wait_stage_mask, Sint64 wait_semaphore, Sint64 signal_semaphore);
```

## Function Parameters

|                                |                      |                                                                                                          |
| ------------------------------ | -------------------- | -------------------------------------------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer**         | the rendering context.                                                                                   |
| Uint32                         | **wait_stage_mask**  | the VkPipelineStageFlags for the wait.                                                                   |
| Sint64                         | **wait_semaphore**   | a VkSempahore to wait on before rendering the current frame, or 0 if not needed.                         |
| Sint64                         | **signal_semaphore** | a VkSempahore that SDL will signal when rendering for the current frame is complete, or 0 if not needed. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The Vulkan renderer will wait for `wait_semaphore` before submitting
rendering commands and signal `signal_semaphore` after rendering commands
are complete for this frame.

This should be called each frame that you want semaphore synchronization.
The Vulkan renderer may have multiple frames in flight on the GPU, so you
should have multiple semaphores that are used for synchronization. Querying
[SDL_PROP_RENDERER_VULKAN_SWAPCHAIN_IMAGE_COUNT_NUMBER](SDL_PROP_RENDERER_VULKAN_SWAPCHAIN_IMAGE_COUNT_NUMBER)
will give you the maximum number of semaphores you'll need.

## Thread Safety

It is **NOT** safe to call this function from two threads at once.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

