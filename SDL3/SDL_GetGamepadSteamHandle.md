# SDL_GetGamepadSteamHandle

Get the Steam Input handle of an opened gamepad, if available.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
Uint64 SDL_GetGamepadSteamHandle(SDL_Gamepad *gamepad);
```

## Function Parameters

|                              |             |                              |
| ---------------------------- | ----------- | ---------------------------- |
| [SDL_Gamepad](SDL_Gamepad) * | **gamepad** | the gamepad object to query. |

## Return Value

([Uint64](Uint64)) Returns the gamepad handle, or 0 if unavailable.

## Remarks

Returns an InputHandle_t for the gamepad that can be used with Steam Input
API: https://partner.steamgames.com/doc/api/ISteamInput

## Version

This function is available since SDL 3.2.0.

## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

