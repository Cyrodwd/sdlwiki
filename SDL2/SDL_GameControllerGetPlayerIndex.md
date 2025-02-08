# SDL_GameControllerGetPlayerIndex

Get the player index of an opened game controller.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
int SDL_GameControllerGetPlayerIndex(SDL_GameController *gamecontroller);
```

## Function Parameters

|                                            |                    |                                      |
| ------------------------------------------ | ------------------ | ------------------------------------ |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | the game controller object to query. |

## Return Value

(int) Returns the player index for controller, or -1 if it's not available.

## Remarks

For XInput controllers this returns the XInput user index.

## Version

This function is available since SDL 2.0.9.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

