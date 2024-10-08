###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HapticUpdateEffect

Update the properties of an effect.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticUpdateEffect(SDL_Haptic * haptic,
                           int effect,
                           SDL_HapticEffect * data);
```

## Function Parameters

|                                        |            |                                                                                                |
| -------------------------------------- | ---------- | ---------------------------------------------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) *             | **haptic** | the [SDL_Haptic](SDL_Haptic) device that has the effect.                                       |
| int                                    | **effect** | the identifier of the effect to update.                                                        |
| [SDL_HapticEffect](SDL_HapticEffect) * | **data**   | an [SDL_HapticEffect](SDL_HapticEffect) structure containing the new effect properties to use. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Can be used dynamically, although behavior when dynamically changing
direction may be strange. Specifically the effect may re-upload itself and
start playing from the start. You also cannot change the type either when
running [SDL_HapticUpdateEffect](SDL_HapticUpdateEffect)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticDestroyEffect](SDL_HapticDestroyEffect)
- [SDL_HapticNewEffect](SDL_HapticNewEffect)
- [SDL_HapticRunEffect](SDL_HapticRunEffect)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

