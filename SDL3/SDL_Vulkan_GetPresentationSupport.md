# SDL_Vulkan_GetPresentationSupport

Query support for presentation via a given physical device and queue family.

## Header File

Defined in [<SDL3/SDL_vulkan.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_vulkan.h)

## Syntax

```c
bool SDL_Vulkan_GetPresentationSupport(VkInstance instance,
                                           VkPhysicalDevice physicalDevice,
                                           Uint32 queueFamilyIndex);
```

## Function Parameters

|                  |                      |                                                           |
| ---------------- | -------------------- | --------------------------------------------------------- |
| VkInstance       | **instance**         | the Vulkan instance handle.                               |
| VkPhysicalDevice | **physicalDevice**   | a valid Vulkan physical device handle.                    |
| [Uint32](Uint32) | **queueFamilyIndex** | a valid queue family index for the given physical device. |

## Return Value

(bool) Returns true if supported, false if unsupported or an error
occurred.

## Remarks

The `instance` must have been created with extensions returned by
[SDL_Vulkan_GetInstanceExtensions](SDL_Vulkan_GetInstanceExtensions)()
enabled.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_Vulkan_GetInstanceExtensions](SDL_Vulkan_GetInstanceExtensions)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVulkan](CategoryVulkan)

