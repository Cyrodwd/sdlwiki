###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetMaxHapticEffects

Get the number of effects a haptic device can store.

## Header File

Defined in [<SDL3/SDL_haptic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_haptic.h)

## Syntax

```c
int SDL_GetMaxHapticEffects(SDL_Haptic *haptic);
```

## Function Parameters

|                            |            |                                               |
| -------------------------- | ---------- | --------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) device to query. |

## Return Value

(int) Returns the number of effects the haptic device can store or a
negative error code on failure; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

On some platforms this isn't fully supported, and therefore is an
approximation. Always check to see if your created effect was actually
created and do not rely solely on
[SDL_GetMaxHapticEffects](SDL_GetMaxHapticEffects)().

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetMaxHapticEffectsPlaying](SDL_GetMaxHapticEffectsPlaying)
- [SDL_GetHapticFeatures](SDL_GetHapticFeatures)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

