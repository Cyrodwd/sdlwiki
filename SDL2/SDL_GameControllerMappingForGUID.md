# SDL_GameControllerMappingForGUID

Get the game controller mapping string for a given GUID.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
char * SDL_GameControllerMappingForGUID(SDL_JoystickGUID guid);
```

## Function Parameters

|                                      |          |                                                                 |
| ------------------------------------ | -------- | --------------------------------------------------------------- |
| [SDL_JoystickGUID](SDL_JoystickGUID) | **guid** | a structure containing the GUID for which a mapping is desired. |

## Return Value

(char *) Returns a mapping string or NULL on error; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The returned string must be freed with [SDL_free](SDL_free)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_JoystickGetDeviceGUID](SDL_JoystickGetDeviceGUID)
- [SDL_JoystickGetGUID](SDL_JoystickGetGUID)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

