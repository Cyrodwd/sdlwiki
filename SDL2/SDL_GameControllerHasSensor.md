###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GameControllerHasSensor

Return whether a game controller has a particular sensor.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
SDL_bool SDL_GameControllerHasSensor(SDL_GameController *gamecontroller, SDL_SensorType type);
```

## Function Parameters

|                                            |                    |                              |
| ------------------------------------------ | ------------------ | ---------------------------- |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | The controller to query.     |
| [SDL_SensorType](SDL_SensorType)           | **type**           | The type of sensor to query. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if the sensor exists,
[SDL_FALSE](SDL_FALSE) otherwise.

## Version

This function is available since SDL 2.0.14.

## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

