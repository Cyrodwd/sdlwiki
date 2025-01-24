# SDL_SetGamepadPlayerIndex

Set the player index of an opened gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
bool SDL_SetGamepadPlayerIndex(SDL_Gamepad *gamepad, int player_index);
```

## Function Parameters

|                              |                  |                                                                                                   |
| ---------------------------- | ---------------- | ------------------------------------------------------------------------------------------------- |
| [SDL_Gamepad](SDL_Gamepad) * | **gamepad**      | the gamepad object to adjust.                                                                     |
| int                          | **player_index** | player index to assign to this gamepad, or -1 to clear the player index and turn off player LEDs. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetGamepadPlayerIndex](SDL_GetGamepadPlayerIndex)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

