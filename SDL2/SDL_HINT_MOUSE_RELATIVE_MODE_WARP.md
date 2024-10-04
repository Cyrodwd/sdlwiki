###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_MOUSE_RELATIVE_MODE_WARP

A variable controlling whether relative mouse mode is implemented using mouse warping

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_MOUSE_RELATIVE_MODE_WARP    "SDL_MOUSE_RELATIVE_MODE_WARP"
```

## Remarks

This variable can be set to the following values:

- "0": Relative mouse mode uses raw input
- "1": Relative mouse mode uses mouse warping

By default SDL will use raw input for relative mouse mode

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

