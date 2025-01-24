# SDL_STANDARD_GRAVITY

A constant to represent standard gravity for accelerometer sensors.

## Header File

Defined in [SDL_sensor.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_sensor.h)

## Syntax

```c
#define SDL_STANDARD_GRAVITY    9.80665f
```

## Remarks

The accelerometer returns the current acceleration in SI meters per second
squared. This measurement includes the force of gravity, so a device at
rest will have an value of [SDL_STANDARD_GRAVITY](SDL_STANDARD_GRAVITY)
away from the center of the earth, which is a positive Y value.





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategorySensor](CategorySensor)

