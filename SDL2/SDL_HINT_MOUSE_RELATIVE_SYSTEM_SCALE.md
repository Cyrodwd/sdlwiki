# SDL_HINT_MOUSE_RELATIVE_SYSTEM_SCALE

A variable controlling whether the system mouse acceleration curve is used for relative mouse motion.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_MOUSE_RELATIVE_SYSTEM_SCALE    "SDL_MOUSE_RELATIVE_SYSTEM_SCALE"
```

## Remarks

This variable can be set to the following values:

- "0": Relative mouse motion will be unscaled (the default)
- "1": Relative mouse motion will be scaled using the system mouse
  acceleration curve.

If
[SDL_HINT_MOUSE_RELATIVE_SPEED_SCALE](SDL_HINT_MOUSE_RELATIVE_SPEED_SCALE)
is set, that will override the system speed scale.

## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

