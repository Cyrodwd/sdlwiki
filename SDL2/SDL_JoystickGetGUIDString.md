# SDL_JoystickGetGUIDString

Get an ASCII string representation for a given [SDL_JoystickGUID](SDL_JoystickGUID).

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
void SDL_JoystickGetGUIDString(SDL_JoystickGUID guid, char *pszGUID, int cbGUID);
```

## Function Parameters

|                                      |             |                                                                         |
| ------------------------------------ | ----------- | ----------------------------------------------------------------------- |
| [SDL_JoystickGUID](SDL_JoystickGUID) | **guid**    | the [SDL_JoystickGUID](SDL_JoystickGUID) you wish to convert to string. |
| char *                               | **pszGUID** | buffer in which to write the ASCII string.                              |
| int                                  | **cbGUID**  | the size of pszGUID.                                                    |

## Remarks

You should supply at least 33 bytes for pszGUID.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_JoystickGetDeviceGUID](SDL_JoystickGetDeviceGUID)
- [SDL_JoystickGetGUID](SDL_JoystickGetGUID)
- [SDL_JoystickGetGUIDFromString](SDL_JoystickGetGUIDFromString)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

