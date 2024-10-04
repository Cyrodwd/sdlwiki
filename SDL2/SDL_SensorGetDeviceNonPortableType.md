###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SensorGetDeviceNonPortableType

Get the platform dependent type of a sensor.

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_sensor.h)

## Syntax

```c
int SDL_SensorGetDeviceNonPortableType(int device_index);
```

## Function Parameters

|     |                  |                      |
| --- | ---------------- | -------------------- |
| int | **device_index** | The sensor to check. |

## Return Value

(int) Returns the sensor platform dependent type, or -1 if `device_index`
is out of range.

## Version

This function is available since SDL 2.0.9.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

