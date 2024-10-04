###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GameControllerGetButton

Get the current state of a button on a game controller.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
Uint8 SDL_GameControllerGetButton(SDL_GameController *gamecontroller,
                                  SDL_GameControllerButton button);
```

## Function Parameters

|                                                      |                    |                                                                                          |
| ---------------------------------------------------- | ------------------ | ---------------------------------------------------------------------------------------- |
| [SDL_GameController](SDL_GameController) *           | **gamecontroller** | a game controller.                                                                       |
| [SDL_GameControllerButton](SDL_GameControllerButton) | **button**         | a button index (one of the [SDL_GameControllerButton](SDL_GameControllerButton) values). |

## Return Value

(Uint8) Returns 1 for pressed state or 0 for not pressed state or error;
call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GameControllerGetAxis](SDL_GameControllerGetAxis)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

