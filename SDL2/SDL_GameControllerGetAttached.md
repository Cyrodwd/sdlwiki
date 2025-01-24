# SDL_GameControllerGetAttached

Check if a controller has been opened and is currently connected.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_bool SDL_GameControllerGetAttached(SDL_GameController *gamecontroller);
```

## Function Parameters

|                                            |                    |                                                                                                         |
| ------------------------------------------ | ------------------ | ------------------------------------------------------------------------------------------------------- |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | a game controller identifier previously returned by [SDL_GameControllerOpen](SDL_GameControllerOpen)(). |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if the controller has
been opened and is currently connected, or [SDL_FALSE](SDL_FALSE) if not.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GameControllerClose](SDL_GameControllerClose)
- [SDL_GameControllerOpen](SDL_GameControllerOpen)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

