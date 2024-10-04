###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_LockJoysticks

Locking for multi-threaded access to the joystick API

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
void SDL_LockJoysticks(void);
```

## Remarks

If you are using the joystick API or handling events from multiple threads
you should use these locking functions to protect access to the joysticks.

In particular, you are guaranteed that the joystick list won't change, so
the API functions that take a joystick index will be valid, and joystick
and game controller events will not be delivered.

As of SDL 2.26.0, you can take the joystick lock around reinitializing the
joystick subsystem, to prevent other threads from seeing joysticks in an
uninitialized state. However, all open joysticks will be closed and SDL
functions called with them will fail.

## Version

This function is available since SDL 2.0.7.

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

