###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_CloseGamepad

Close a gamepad previously opened with [SDL_OpenGamepad](SDL_OpenGamepad)().

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
void SDL_CloseGamepad(SDL_Gamepad *gamepad);
```

## Function Parameters

|                              |             |                                                                                   |
| ---------------------------- | ----------- | --------------------------------------------------------------------------------- |
| [SDL_Gamepad](SDL_Gamepad) * | **gamepad** | a gamepad identifier previously returned by [SDL_OpenGamepad](SDL_OpenGamepad)(). |

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_OpenGamepad](SDL_OpenGamepad)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

