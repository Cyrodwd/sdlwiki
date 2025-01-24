# SDL_GameControllerGetSensorData

Get the current state of a game controller sensor.

## Header File

Defined in [SDL_gamecontroller.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gamecontroller.h)

## Syntax

```c
int SDL_GameControllerGetSensorData(SDL_GameController *gamecontroller, SDL_SensorType type, float *data, int num_values);
```

## Function Parameters

|                                            |                    |                                                 |
| ------------------------------------------ | ------------------ | ----------------------------------------------- |
| [SDL_GameController](SDL_GameController) * | **gamecontroller** | The controller to query.                        |
| [SDL_SensorType](SDL_SensorType)           | **type**           | The type of sensor to query.                    |
| float *                                    | **data**           | A pointer filled with the current sensor state. |
| int                                        | **num_values**     | The number of values to write to data.          |

## Return Value

(int) Return 0 or -1 if an error occurred.

## Remarks

The number of values and interpretation of the data is sensor dependent.
See [SDL_sensor](SDL_sensor).h for the details for each type of sensor.

## Version

This function is available since SDL 2.0.14.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGameController](CategoryGameController)

