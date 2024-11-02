###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetHapticFeatures

Get the haptic device's supported features in bitwise manner.

## Header File

Defined in [<SDL3/SDL_haptic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_haptic.h)

## Syntax

```c
Uint32 SDL_GetHapticFeatures(SDL_Haptic *haptic);
```

## Function Parameters

|                            |            |                                               |
| -------------------------- | ---------- | --------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) device to query. |

## Return Value

([Uint32](Uint32)) Returns a list of supported haptic features in bitwise
manner (OR'd), or 0 on failure; call [SDL_GetError](SDL_GetError)() for
more information.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_HapticEffectSupported](SDL_HapticEffectSupported)
- [SDL_GetMaxHapticEffects](SDL_GetMaxHapticEffects)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

