# SDL_HapticDestroyEffect

Destroy a haptic effect on the device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
void SDL_HapticDestroyEffect(SDL_Haptic * haptic,
                             int effect);
```

## Function Parameters

|                            |            |                                                               |
| -------------------------- | ---------- | ------------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) device to destroy the effect on. |
| int                        | **effect** | the ID of the haptic effect to destroy.                       |

## Remarks

This will stop the effect if it's running. Effects are automatically
destroyed when the device is closed.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticNewEffect](SDL_HapticNewEffect)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

