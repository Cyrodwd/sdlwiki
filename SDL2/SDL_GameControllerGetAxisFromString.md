# SDL_GameControllerGetAxisFromString

Convert a string into [SDL_GameControllerAxis](SDL_GameControllerAxis) enum.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_GameControllerAxis SDL_GameControllerGetAxisFromString(const char *str);
```

## Function Parameters

|              |         |                                                                      |
| ------------ | ------- | -------------------------------------------------------------------- |
| const char * | **str** | string representing a [SDL_GameController](SDL_GameController) axis. |

## Return Value

([SDL_GameControllerAxis](SDL_GameControllerAxis)) Returns the
[SDL_GameControllerAxis](SDL_GameControllerAxis) enum corresponding to the
input string, or
[`SDL_CONTROLLER_AXIS_INVALID`](SDL_CONTROLLER_AXIS_INVALID) if no match
was found.

## Remarks

This function is called internally to translate
[SDL_GameController](SDL_GameController) mapping strings for the underlying
joystick device into the consistent
[SDL_GameController](SDL_GameController) mapping. You do not normally need
to call this function unless you are parsing
[SDL_GameController](SDL_GameController) mappings in your own code.

Note specially that "righttrigger" and "lefttrigger" map to
[`SDL_CONTROLLER_AXIS_TRIGGERRIGHT`](SDL_CONTROLLER_AXIS_TRIGGERRIGHT) and
[`SDL_CONTROLLER_AXIS_TRIGGERLEFT`](SDL_CONTROLLER_AXIS_TRIGGERLEFT),
respectively.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GameControllerGetStringForAxis](SDL_GameControllerGetStringForAxis)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

