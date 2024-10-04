###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_EMSCRIPTEN_ASYNCIFY

Disable giving back control to the browser automatically when running with asyncify

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_EMSCRIPTEN_ASYNCIFY   "SDL_EMSCRIPTEN_ASYNCIFY"
```

## Remarks

With -s ASYNCIFY, SDL2 calls emscripten_sleep during operations such as
refreshing the screen or polling events.

This hint only applies to the emscripten platform

The variable can be set to the following values:

- "0": Disable emscripten_sleep calls (if you give back browser control
  manually or use asyncify for other purposes)
- "1": Enable emscripten_sleep calls (the default)

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

