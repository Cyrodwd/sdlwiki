###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HapticSetAutocenter

Set the global autocenter of the device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticSetAutocenter(SDL_Haptic * haptic,
                            int autocenter);
```

## Function Parameters

|                            |                |                                                              |
| -------------------------- | -------------- | ------------------------------------------------------------ |
| [SDL_Haptic](SDL_Haptic) * | **haptic**     | the [SDL_Haptic](SDL_Haptic) device to set autocentering on. |
| int                        | **autocenter** | value to set autocenter to (0-100).                          |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Autocenter should be between 0 and 100. Setting it to 0 will disable
autocentering.

Device must support the [SDL_HAPTIC_AUTOCENTER](SDL_HAPTIC_AUTOCENTER)
feature.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticQuery](SDL_HapticQuery)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

