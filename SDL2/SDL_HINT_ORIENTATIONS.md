###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_ORIENTATIONS

A variable controlling which orientations are allowed on iOS/Android.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_ORIENTATIONS "SDL_IOS_ORIENTATIONS"
```

## Remarks

In some circumstances it is necessary to be able to explicitly control
which UI orientations are allowed.

This variable is a space delimited list of the following values:

- "LandscapeLeft"
- "LandscapeRight"
- "Portrait"
- "PortraitUpsideDown"

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

