###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
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

(Uint16) Return the controller firmware version, or zero if unavailable.

## Remarks

If the firmware version isn't available this function returns 0.

## Version

This function is available since SDL 2.24.0.

## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

