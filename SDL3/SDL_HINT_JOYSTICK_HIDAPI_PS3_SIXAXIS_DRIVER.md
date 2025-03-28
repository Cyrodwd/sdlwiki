# SDL_HINT_JOYSTICK_HIDAPI_PS3_SIXAXIS_DRIVER

A variable controlling whether the Sony driver (sixaxis.sys) for PS3 controllers (Sixaxis/DualShock 3) should be used.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_HIDAPI_PS3_SIXAXIS_DRIVER "SDL_JOYSTICK_HIDAPI_PS3_SIXAXIS_DRIVER"
```

## Remarks

The variable can be set to the following values:

- "0": Sony driver (sixaxis.sys) is not used.
- "1": Sony driver (sixaxis.sys) is used.

The default value is 0.

This hint should be set before initializing joysticks and gamepads.

## Version

This hint is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

