###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_Vulkan_GetVkGetInstanceProcAddr

Get the address of the `vkGetInstanceProcAddr` function.

## Header File

Defined in [<SDL3/SDL_vulkan.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_vulkan.h)

## Syntax

```c
SDL_FunctionPointer SDL_Vulkan_GetVkGetInstanceProcAddr(void);
```

## Return Value

([SDL_FunctionPointer](SDL_FunctionPointer)) Returns the function pointer
for `vkGetInstanceProcAddr` or NULL on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This should be called after either calling
[SDL_Vulkan_LoadLibrary](SDL_Vulkan_LoadLibrary)() or creating an
[SDL_Window](SDL_Window) with the [`SDL_WINDOW_VULKAN`](SDL_WINDOW_VULKAN)
flag.

The actual type of the returned function pointer is
PFN_vkGetInstanceProcAddr, but that isn't available because the Vulkan
headers are not included here. You should cast the return value of this
function to that type, e.g.

`vkGetInstanceProcAddr =
(PFN_vkGetInstanceProcAddr)SDL_Vulkan_GetVkGetInstanceProcAddr();`

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVulkan](CategoryVulkan)

