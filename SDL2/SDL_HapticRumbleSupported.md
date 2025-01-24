# SDL_HapticRumbleSupported

Check whether rumble is supported on a haptic device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_HapticRumbleSupported(SDL_Haptic * haptic);
```

## Function Parameters

|                            |            |                                            |
| -------------------------- | ---------- | ------------------------------------------ |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | haptic device to check for rumble support. |

## Return Value

(int) Returns [SDL_TRUE](SDL_TRUE) if effect is supported,
[SDL_FALSE](SDL_FALSE) if it isn't, or a negative error code on failure;
call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticRumbleInit](SDL_HapticRumbleInit)
- [SDL_HapticRumblePlay](SDL_HapticRumblePlay)
- [SDL_HapticRumbleStop](SDL_HapticRumbleStop)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

