###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_HINT_RENDER_METAL_PREFER_LOW_POWER_DEVICE

A variable controlling whether the Metal render driver select low power device over default one.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_RENDER_METAL_PREFER_LOW_POWER_DEVICE "SDL_RENDER_METAL_PREFER_LOW_POWER_DEVICE"
```

## Remarks

The variable can be set to the following values:

- "0": Use the preferred OS device. (default)
- "1": Select a low power device.

This hint should be set before creating a renderer.

## Version

This hint is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

