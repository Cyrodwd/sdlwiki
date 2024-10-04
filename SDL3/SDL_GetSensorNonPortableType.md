###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetSensorNonPortableType

Get the platform dependent type of a sensor.

## Header File

Defined in [<SDL3/SDL_sensor.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_sensor.h)

## Syntax

```c
int SDL_GetSensorNonPortableType(SDL_Sensor *sensor);
```

## Function Parameters

|                            |            |                                                 |
| -------------------------- | ---------- | ----------------------------------------------- |
| [SDL_Sensor](SDL_Sensor) * | **sensor** | the [SDL_Sensor](SDL_Sensor) object to inspect. |

## Return Value

(int) Returns the sensor platform dependent type, or -1 if `sensor` is
NULL.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

