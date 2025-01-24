# SDL_GetHapticName

Get the implementation dependent name of a haptic device.

## Header File

Defined in [<SDL3/SDL_haptic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_haptic.h)

## Syntax

```c
const char * SDL_GetHapticName(SDL_Haptic *haptic);
```

## Function Parameters

|                            |            |                                                                                    |
| -------------------------- | ---------- | ---------------------------------------------------------------------------------- |
| [SDL_Haptic](SDL_Haptic) * | **haptic** | the [SDL_Haptic](SDL_Haptic) obtained from [SDL_OpenJoystick](SDL_OpenJoystick)(). |

## Return Value

(const char *) Returns the name of the selected haptic device. If no name
can be found, this function returns NULL; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetHapticNameForID](SDL_GetHapticNameForID)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

