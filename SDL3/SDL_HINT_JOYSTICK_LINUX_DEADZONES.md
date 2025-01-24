# SDL_HINT_JOYSTICK_LINUX_DEADZONES

A variable controlling whether joysticks on Linux adhere to their HID-defined deadzones or return unfiltered values.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_LINUX_DEADZONES "SDL_JOYSTICK_LINUX_DEADZONES"
```

## Remarks

The variable can be set to the following values:

- "0": Return unfiltered joystick axis values. (default)
- "1": Return axis values with deadzones taken into account.

This hint should be set before a controller is opened.

## Version

This hint is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

