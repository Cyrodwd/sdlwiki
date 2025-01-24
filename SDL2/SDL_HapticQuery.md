# SDL_HapticQuery

Get the haptic device's supported features in bitwise manner.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
unsigned int SDL_HapticQuery(SDL_Haptic * haptic);
```

## Function Parameters

|                            |            |                                               |
| -------------------------- | ---------- | --------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) device to query. |

## Return Value

(unsigned int) Returns a list of supported haptic features in bitwise
manner (OR'd), or 0 on failure; call [SDL_GetError](SDL_GetError)() for
more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticEffectSupported](SDL_HapticEffectSupported)
- [SDL_HapticNumEffects](SDL_HapticNumEffects)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

