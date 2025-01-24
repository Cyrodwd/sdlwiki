# SDL_JoystickFromInstanceID

Get the [SDL_Joystick](SDL_Joystick) associated with an instance id.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
SDL_Joystick* SDL_JoystickFromInstanceID(SDL_JoystickID instance_id);
```

## Function Parameters

|                                  |                 |                                                              |
| -------------------------------- | --------------- | ------------------------------------------------------------ |
| [SDL_JoystickID](SDL_JoystickID) | **instance_id** | the instance id to get the [SDL_Joystick](SDL_Joystick) for. |

## Return Value

([SDL_Joystick](SDL_Joystick) *) Returns an [SDL_Joystick](SDL_Joystick) on
success or NULL on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Version

This function is available since SDL 2.0.4.

## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

