###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GameControllerGetButtonFromString

Convert a string into an [SDL_GameControllerButton](SDL_GameControllerButton) enum.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_GameControllerButton SDL_GameControllerGetButtonFromString(const char *str);
```

## Function Parameters

|              |         |                                                                      |
| ------------ | ------- | -------------------------------------------------------------------- |
| const char * | **str** | string representing a [SDL_GameController](SDL_GameController) axis. |

## Return Value

([SDL_GameControllerButton](SDL_GameControllerButton)) Returns the
[SDL_GameControllerButton](SDL_GameControllerButton) enum corresponding to
the input string, or
[`SDL_CONTROLLER_AXIS_INVALID`](SDL_CONTROLLER_AXIS_INVALID) if no match
was found.

## Remarks

This function is called internally to translate
[SDL_GameController](SDL_GameController) mapping strings for the underlying
joystick device into the consistent
[SDL_GameController](SDL_GameController) mapping. You do not normally need
to call this function unless you are parsing
[SDL_GameController](SDL_GameController) mappings in your own code.

## Version

This function is available since SDL 2.0.0.

## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

