# SDL_GetJoystickProductForID

Get the USB product ID of a joystick, if available.

## Header File

Defined in [<SDL3/SDL_joystick.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_joystick.h)

## Syntax

```c
Uint16 SDL_GetJoystickProductForID(SDL_JoystickID instance_id);
```

## Function Parameters

|                                  |                 |                           |
| -------------------------------- | --------------- | ------------------------- |
| [SDL_JoystickID](SDL_JoystickID) | **instance_id** | the joystick instance ID. |

## Return Value

([Uint16](Uint16)) Returns the USB product ID of the selected joystick. If
called with an invalid instance_id, this function returns 0.

## Remarks

This can be called before any joysticks are opened. If the product ID isn't
available this function returns 0.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetJoystickProduct](SDL_GetJoystickProduct)
- [SDL_GetJoysticks](SDL_GetJoysticks)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

