# SDL_JoystickGetSerial

Get the serial number of an opened joystick, if available.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
const char * SDL_JoystickGetSerial(SDL_Joystick *joystick);
```

## Function Parameters

|                                |              |                                                                                        |
| ------------------------------ | ------------ | -------------------------------------------------------------------------------------- |
| [SDL_Joystick](SDL_Joystick) * | **joystick** | the [SDL_Joystick](SDL_Joystick) obtained from [SDL_JoystickOpen](SDL_JoystickOpen)(). |

## Return Value

(const char *) Returns the serial number of the selected joystick, or NULL
if unavailable.

## Remarks

Returns the serial number of the joystick, or NULL if it is not available.

## Version

This function is available since SDL 2.0.14.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

