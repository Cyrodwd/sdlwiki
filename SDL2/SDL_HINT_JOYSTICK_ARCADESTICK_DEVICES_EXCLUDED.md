###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_JOYSTICK_ARCADESTICK_DEVICES_EXCLUDED

A variable containing a list of devices that are not arcade stick style controllers.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_ARCADESTICK_DEVICES_EXCLUDED "SDL_JOYSTICK_ARCADESTICK_DEVICES_EXCLUDED"
```

## Remarks

This will override
[SDL_HINT_JOYSTICK_ARCADESTICK_DEVICES](SDL_HINT_JOYSTICK_ARCADESTICK_DEVICES)
and the built in device list.

The format of the string is a comma separated list of USB VID/PID pairs in
hexadecimal form, e.g.

0xAAAA/0xBBBB,0xCCCC/0xDDDD

The variable can also take the form of @file, in which case the named file
will be loaded and interpreted as the value of the variable.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

