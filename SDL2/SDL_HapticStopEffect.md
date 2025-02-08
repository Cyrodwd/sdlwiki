# SDL_HapticStopEffect

Stop the haptic effect on its associated haptic device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticStopEffect(SDL_Haptic * haptic,
                         int effect);
```

## Function Parameters

|                            |            |                                                            |
| -------------------------- | ---------- | ---------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) device to stop the effect on. |
| int                        | **effect** | the ID of the haptic effect to stop.                       |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

*

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticDestroyEffect](SDL_HapticDestroyEffect)
- [SDL_HapticRunEffect](SDL_HapticRunEffect)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

