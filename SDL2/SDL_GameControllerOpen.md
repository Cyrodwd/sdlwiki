# SDL_GameControllerOpen

Open a game controller for use.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_GameController* SDL_GameControllerOpen(int joystick_index);
```

## Function Parameters

|     |                    |                                                                             |
| --- | ------------------ | --------------------------------------------------------------------------- |
| int | **joystick_index** | the device_index of a device, up to [SDL_NumJoysticks](SDL_NumJoysticks)(). |

## Return Value

([SDL_GameController](SDL_GameController) *) Returns a gamecontroller
identifier or NULL if an error occurred; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

`joystick_index` is the same as the `device_index` passed to
[SDL_JoystickOpen](SDL_JoystickOpen)().

The index passed as an argument refers to the N'th game controller on the
system. This index is not the value which will identify this controller in
future controller events. The joystick's instance id
([SDL_JoystickID](SDL_JoystickID)) will be used there instead.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GameControllerClose](SDL_GameControllerClose)
- [SDL_GameControllerNameForIndex](SDL_GameControllerNameForIndex)
- [SDL_IsGameController](SDL_IsGameController)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

