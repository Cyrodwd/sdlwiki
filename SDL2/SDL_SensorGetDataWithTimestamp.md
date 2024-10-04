###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SensorGetDataWithTimestamp

Get the current state of an opened sensor with the timestamp of the last update.

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_sensor.h)

## Syntax

```c
int SDL_SensorGetDataWithTimestamp(SDL_Sensor *sensor, Uint64 *timestamp, float *data, int num_values);
```

## Function Parameters

|                            |                |                                                                                                              |
| -------------------------- | -------------- | ------------------------------------------------------------------------------------------------------------ |
| [SDL_Sensor](SDL_Sensor) * | **sensor**     | The [SDL_Sensor](SDL_Sensor) object to query.                                                                |
| Uint64 *                   | **timestamp**  | A pointer filled with the timestamp in microseconds of the current sensor reading if available, or 0 if not. |
| float *                    | **data**       | A pointer filled with the current sensor state.                                                              |
| int                        | **num_values** | The number of values to write to data.                                                                       |

## Return Value

(int) Returns 0 or -1 if an error occurred.

## Remarks

The number of values and interpretation of the data is sensor dependent.

## Version

This function is available since SDL 2.26.0.

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

