###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HapticGetEffectStatus

Get the status of the current effect on the specified haptic device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticGetEffectStatus(SDL_Haptic * haptic,
                          int effect);
```

## Function Parameters

|                            |            |                                                                        |
| -------------------------- | ---------- | ---------------------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) device to query for the effect status on. |
| int                        | **effect** | the ID of the haptic effect to query its status.                       |

## Return Value

(int) Returns 0 if it isn't playing, 1 if it is playing, or a negative
error code on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

Device must support the [SDL_HAPTIC_STATUS](SDL_HAPTIC_STATUS) feature.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticRunEffect](SDL_HapticRunEffect)
- [SDL_HapticStopEffect](SDL_HapticStopEffect)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

