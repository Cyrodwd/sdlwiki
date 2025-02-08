# SDL_GameControllerGetBindForAxis

Get the SDL joystick layer binding for a controller axis mapping.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
extern DECLSPEC SDL_GameControllerButtonBind SDLCALL
SDL_GameControllerGetBindForAxis(SDL_GameController *gamecontroller,
                                 SDL_GameControllerAxis axis);
```

## Function Parameters

|                                                  |                    |                                                                                          |
| ------------------------------------------------ | ------------------ | ---------------------------------------------------------------------------------------- |
| [SDL_GameController](SDL_GameController) *       | **gamecontroller** | a game controller.                                                                       |
| [SDL_GameControllerAxis](SDL_GameControllerAxis) | **axis**           | an axis enum value (one of the [SDL_GameControllerAxis](SDL_GameControllerAxis) values). |

## Return Value

([SDL_GameControllerButtonBind](SDL_GameControllerButtonBind)) Returns a
[SDL_GameControllerButtonBind](SDL_GameControllerButtonBind) describing the
bind. On failure (like the given Controller axis doesn't exist on the
device), its `.bindType` will be
[`SDL_CONTROLLER_BINDTYPE_NONE`](SDL_CONTROLLER_BINDTYPE_NONE).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GameControllerGetBindForButton](SDL_GameControllerGetBindForButton)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

