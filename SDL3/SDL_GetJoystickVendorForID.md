# SDL_GetJoystickVendorForID

Get the USB vendor ID of a joystick, if available.

## Header File

Defined in [<SDL3/SDL_joystick.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_joystick.h)

## Syntax

```c
Uint16 SDL_GetJoystickVendorForID(SDL_JoystickID instance_id);
```

## Function Parameters

|                                  |                 |                           |
| -------------------------------- | --------------- | ------------------------- |
| [SDL_JoystickID](SDL_JoystickID) | **instance_id** | the joystick instance ID. |

## Return Value

([Uint16](Uint16)) Returns the USB vendor ID of the selected joystick. If
called with an invalid instance_id, this function returns 0.

## Remarks

This can be called before any joysticks are opened. If the vendor ID isn't
available this function returns 0.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetJoystickVendor](SDL_GetJoystickVendor)
- [SDL_GetJoysticks](SDL_GetJoysticks)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

