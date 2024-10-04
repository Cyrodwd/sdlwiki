###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GameControllerSendEffect

Send a controller specific effect packet

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
int SDL_GameControllerSendEffect(SDL_GameController *gamecontroller, const void *data, int size);
```

## Function Parameters

|                                            |                    |                                                 |
| ------------------------------------------ | ------------------ | ----------------------------------------------- |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | The controller to affect.                       |
| const void *                               | **data**           | The data to send to the controller.             |
| int                                        | **size**           | The size of the data to send to the controller. |

## Return Value

(int) Returns 0, or -1 if this controller or driver doesn't support effect
packets.

## Version

This function is available since SDL 2.0.16.

## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

