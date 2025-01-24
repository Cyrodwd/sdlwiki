# SDL_GetSensorProperties

Get the properties associated with a sensor.

## Header File

Defined in [<SDL3/SDL_sensor.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_sensor.h)

## Syntax

```c
SDL_PropertiesID SDL_GetSensorProperties(SDL_Sensor *sensor);
```

## Function Parameters

|                            |            |                                      |
| -------------------------- | ---------- | ------------------------------------ |
| [SDL_Sensor](SDL_Sensor) * | **sensor** | the [SDL_Sensor](SDL_Sensor) object. |

## Return Value

([SDL_PropertiesID](SDL_PropertiesID)) Returns a valid property ID on
success or 0 on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

