# SDL_GetGamepadNameForID

Get the implementation dependent name of a gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
const char * SDL_GetGamepadNameForID(SDL_JoystickID instance_id);
```

## Function Parameters

|                                  |                 |                           |
| -------------------------------- | --------------- | ------------------------- |
| [SDL_JoystickID](SDL_JoystickID) | **instance_id** | the joystick instance ID. |

## Return Value

(const char *) Returns the name of the selected gamepad. If no name can be
found, this function returns NULL; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

This can be called before any gamepads are opened.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetGamepadName](SDL_GetGamepadName)
- [SDL_GetGamepads](SDL_GetGamepads)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

