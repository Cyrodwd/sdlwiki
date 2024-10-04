###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SensorUpdate

Update the current state of the open sensors.

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_sensor.h)

## Syntax

```c
void SDL_SensorUpdate(void);
```

## Remarks

This is called automatically by the event loop if sensor events are
enabled.

This needs to be called from the thread that initialized the sensor
subsystem.

## Version

This function is available since SDL 2.0.9.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySensor](CategorySensor)

