###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_VIDEO_WAYLAND_ALLOW_LIBDECOR

A variable controlling whether the libdecor Wayland backend is allowed to be used.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_VIDEO_WAYLAND_ALLOW_LIBDECOR "SDL_VIDEO_WAYLAND_ALLOW_LIBDECOR"
```

## Remarks

This variable can be set to the following values:

- "0": libdecor use is disabled.
- "1": libdecor use is enabled (default).

libdecor is used over xdg-shell when xdg-decoration protocol is
unavailable.

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

