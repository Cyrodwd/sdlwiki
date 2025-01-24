# SDL_HapticRumbleStop

Stop the simple rumble on a haptic device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticRumbleStop(SDL_Haptic * haptic);
```

## Function Parameters

|                            |            |                                                 |
| -------------------------- | ---------- | ----------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the haptic device to stop the rumble effect on. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticRumbleInit](SDL_HapticRumbleInit)
- [SDL_HapticRumblePlay](SDL_HapticRumblePlay)
- [SDL_HapticRumbleSupported](SDL_HapticRumbleSupported)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

