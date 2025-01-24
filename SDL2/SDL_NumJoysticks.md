# SDL_NumJoysticks

Count the number of joysticks attached to the system.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
int SDL_NumJoysticks(void);
```

## Return Value

(int) Returns the number of attached joysticks on success or a negative
error code on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_JoystickName](SDL_JoystickName)
- [SDL_JoystickPath](SDL_JoystickPath)
- [SDL_JoystickOpen](SDL_JoystickOpen)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

