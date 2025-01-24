# SDL_JoystickGetButton

Get the current state of a button on a joystick.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
Uint8 SDL_JoystickGetButton(SDL_Joystick *joystick,
                            int button);
```

## Function Parameters

|                                |              |                                                                            |
| ------------------------------ | ------------ | -------------------------------------------------------------------------- |
| [SDL_Joystick](SDL_Joystick) * | **joystick** | an [SDL_Joystick](SDL_Joystick) structure containing joystick information. |
| int                            | **button**   | the button index to get the state from; indices start at index 0.          |

## Return Value

(Uint8) Returns 1 if the specified button is pressed, 0 otherwise.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_JoystickNumButtons](SDL_JoystickNumButtons)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

