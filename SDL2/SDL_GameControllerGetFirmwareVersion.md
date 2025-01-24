# SDL_GameControllerGetFirmwareVersion

Get the firmware version of an opened controller, if available.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
Uint16 SDL_GameControllerGetFirmwareVersion(SDL_GameController *gamecontroller);
```

## Function Parameters

|                                            |                    |                                      |
| ------------------------------------------ | ------------------ | ------------------------------------ |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | the game controller object to query. |

## Return Value

([Uint16](Uint16)) Return the controller firmware version, or zero if
unavailable.

## Remarks

If the firmware version isn't available this function returns 0.

## Version

This function is available since SDL 2.24.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

