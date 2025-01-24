# SDL_HapticRumbleInit

Initialize a haptic device for simple rumble playback.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticRumbleInit(SDL_Haptic * haptic);
```

## Function Parameters

|                            |            |                                                             |
| -------------------------- | ---------- | ----------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the haptic device to initialize for simple rumble playback. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticOpen](SDL_HapticOpen)
- [SDL_HapticRumblePlay](SDL_HapticRumblePlay)
- [SDL_HapticRumbleStop](SDL_HapticRumbleStop)
- [SDL_HapticRumbleSupported](SDL_HapticRumbleSupported)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

