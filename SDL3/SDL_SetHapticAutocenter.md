###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_SetHapticAutocenter

Set the global autocenter of the device.

## Header File

Defined in [<SDL3/SDL_haptic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_haptic.h)

## Syntax

```c
bool SDL_SetHapticAutocenter(SDL_Haptic *haptic, int autocenter);
```

## Function Parameters

|                            |                |                                                              |
| -------------------------- | -------------- | ------------------------------------------------------------ |
| [SDL_Haptic](SDL_Haptic) * | **haptic**     | the [SDL_Haptic](SDL_Haptic) device to set autocentering on. |
| int                        | **autocenter** | value to set autocenter to (0-100).                          |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Autocenter should be between 0 and 100. Setting it to 0 will disable
autocentering.

Device must support the [SDL_HAPTIC_AUTOCENTER](SDL_HAPTIC_AUTOCENTER)
feature.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetHapticFeatures](SDL_GetHapticFeatures)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

