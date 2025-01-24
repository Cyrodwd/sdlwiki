# SDL_SensorGetInstanceID

Get the instance ID of a sensor.

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_sensor.h)

## Syntax

```c
SDL_SensorID SDL_SensorGetInstanceID(SDL_Sensor *sensor);
```

## Function Parameters

|                            |            |                                                 |
| -------------------------- | ---------- | ----------------------------------------------- |
| [SDL_Sensor](SDL_Sensor) * | **sensor** | The [SDL_Sensor](SDL_Sensor) object to inspect. |

## Return Value

([SDL_SensorID](SDL_SensorID)) Returns the sensor instance ID, or -1 if
`sensor` is NULL.

## Version

This function is available since SDL 2.0.9.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

