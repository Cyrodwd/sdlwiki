###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetGamepadPlayerIndex

Get the player index of an opened gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
int SDL_GetGamepadPlayerIndex(SDL_Gamepad *gamepad);
```

## Function Parameters

|                              |             |                              |
| ---------------------------- | ----------- | ---------------------------- |
| [SDL_Gamepad](SDL_Gamepad) * | **gamepad** | the gamepad object to query. |

## Return Value

(int) Returns the player index for gamepad, or -1 if it's not available.

## Remarks

For XInput gamepads this returns the XInput user index.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_SetGamepadPlayerIndex](SDL_SetGamepadPlayerIndex)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

