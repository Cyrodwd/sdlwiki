###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_JOYSTICK_HIDAPI_COMBINE_JOY_CONS

A variable controlling whether Nintendo Switch Joy-Con controllers will be combined into a single Pro-like controller when using the HIDAPI driver

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_HIDAPI_COMBINE_JOY_CONS "SDL_JOYSTICK_HIDAPI_COMBINE_JOY_CONS"
```

## Remarks

This variable can be set to the following values:

- "0": Left and right Joy-Con controllers will not be combined and each
  will be a mini-gamepad
- "1": Left and right Joy-Con controllers will be combined into a single
  controller (the default)

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

