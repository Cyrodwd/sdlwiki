###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HapticNumEffects

Get the number of effects a haptic device can store.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticNumEffects(SDL_Haptic * haptic);
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
[SDL_HapticNumEffects](SDL_HapticNumEffects)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticNumEffectsPlaying](SDL_HapticNumEffectsPlaying)
- [SDL_HapticQuery](SDL_HapticQuery)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

