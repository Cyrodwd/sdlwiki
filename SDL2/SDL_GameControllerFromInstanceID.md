# SDL_GameControllerFromInstanceID

Get the [SDL_GameController](SDL_GameController) associated with an instance id.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_GameController* SDL_GameControllerFromInstanceID(SDL_JoystickID joyid);
```

## Function Parameters

|                                  |           |                                                                          |
| -------------------------------- | --------- | ------------------------------------------------------------------------ |
| [SDL_JoystickID](SDL_JoystickID) | **joyid** | the instance id to get the [SDL_GameController](SDL_GameController) for. |

## Return Value

([SDL_GameController](SDL_GameController) *) Returns an
[SDL_GameController](SDL_GameController) on success or NULL on failure;
call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.4.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

