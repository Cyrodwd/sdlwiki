# SDL_SensorGetType

Get the type of a sensor.

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_sensor.h)

## Syntax

```c
SDL_SensorType SDL_SensorGetType(SDL_Sensor *sensor);
```

## Function Parameters

|                            |            |                                                 |
| -------------------------- | ---------- | ----------------------------------------------- |
| [SDL_Sensor](SDL_Sensor) * | **sensor** | The [SDL_Sensor](SDL_Sensor) object to inspect. |

## Return Value

([SDL_SensorType](SDL_SensorType)) Returns the
[SDL_SensorType](SDL_SensorType) type, or
[`SDL_SENSOR_INVALID`](SDL_SENSOR_INVALID) if `sensor` is NULL.

## Version

This function is available since SDL 2.0.9.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

