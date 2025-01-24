# SDL_GameControllerFromPlayerIndex

Get the [SDL_GameController](SDL_GameController) associated with a player index.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_GameController* SDL_GameControllerFromPlayerIndex(int player_index);
```

## Function Parameters

|     |                  |                                                                     |
| --- | ---------------- | ------------------------------------------------------------------- |
| int | **player_index** | the player index, which is not the device index or the instance id! |

## Return Value

([SDL_GameController](SDL_GameController) *) Returns the
[SDL_GameController](SDL_GameController) associated with a player index.

## Remarks

Please note that the player index is _not_ the device index, nor is it the
instance id!

## Version

This function is available since SDL 2.0.12.

## See Also

- [SDL_GameControllerGetPlayerIndex](SDL_GameControllerGetPlayerIndex)
- [SDL_GameControllerSetPlayerIndex](SDL_GameControllerSetPlayerIndex)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

