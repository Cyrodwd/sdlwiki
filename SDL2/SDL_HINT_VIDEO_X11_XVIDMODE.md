# SDL_HINT_VIDEO_X11_XVIDMODE

A no-longer-used variable controlling whether the X11 VidMode extension should be used.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_VIDEO_X11_XVIDMODE         "SDL_VIDEO_X11_XVIDMODE"
```

## Remarks

Before SDL 2.0.24, this would let apps and users disable XVidMode support
on X11. Now SDL never uses XVidMode, and does not check for this hint at
all. The preprocessor define is left here for source compatibility.

## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

