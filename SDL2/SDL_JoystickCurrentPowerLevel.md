# SDL_JoystickCurrentPowerLevel

Get the battery level of a joystick as [SDL_JoystickPowerLevel](SDL_JoystickPowerLevel).

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
SDL_JoystickPowerLevel SDL_JoystickCurrentPowerLevel(SDL_Joystick *joystick);
```

## Function Parameters

|                                |              |                                            |
| ------------------------------ | ------------ | ------------------------------------------ |
| [SDL_Joystick](SDL_Joystick) * | **joystick** | the [SDL_Joystick](SDL_Joystick) to query. |

## Return Value

([SDL_JoystickPowerLevel](SDL_JoystickPowerLevel)) Returns the current
battery level as [SDL_JoystickPowerLevel](SDL_JoystickPowerLevel) on
success or [`SDL_JOYSTICK_POWER_UNKNOWN`](SDL_JOYSTICK_POWER_UNKNOWN) if it
is unknown.

## Version

This function is available since SDL 2.0.4.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

