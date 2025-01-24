# SDL_HINT_JOYSTICK_THREAD

A variable controlling whether a separate thread should be used for handling joystick detection and raw input messages on Windows

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_THREAD "SDL_JOYSTICK_THREAD"
```

## Remarks

This variable can be set to the following values:

- "0": A separate thread is not used (the default)
- "1": A separate thread is used for handling raw input messages





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

