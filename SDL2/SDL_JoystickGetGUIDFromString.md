# SDL_JoystickGetGUIDFromString

Convert a GUID string into a [SDL_JoystickGUID](SDL_JoystickGUID) structure.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
SDL_JoystickGUID SDL_JoystickGetGUIDFromString(const char *pchGUID);
```

## Function Parameters

|              |             |                                                      |
| ------------ | ----------- | ---------------------------------------------------- |
| const char * | **pchGUID** | string containing an ASCII representation of a GUID. |

## Return Value

([SDL_JoystickGUID](SDL_JoystickGUID)) Returns a
[SDL_JoystickGUID](SDL_JoystickGUID) structure.

## Remarks

Performs no error checking. If this function is given a string containing
an invalid GUID, the function will silently succeed, but the GUID generated
will not be useful.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_JoystickGetGUIDString](SDL_JoystickGetGUIDString)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

