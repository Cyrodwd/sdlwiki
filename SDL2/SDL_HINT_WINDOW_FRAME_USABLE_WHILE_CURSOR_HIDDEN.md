###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_WINDOW_FRAME_USABLE_WHILE_CURSOR_HIDDEN

A variable controlling whether the window frame and title bar are interactive when the cursor is hidden

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_WINDOW_FRAME_USABLE_WHILE_CURSOR_HIDDEN    "SDL_WINDOW_FRAME_USABLE_WHILE_CURSOR_HIDDEN"
```

## Remarks

This variable can be set to the following values:

- "0": The window frame is not interactive when the cursor is hidden (no
  move, resize, etc)
- "1": The window frame is interactive when the cursor is hidden

By default SDL will allow interaction with the window frame when the cursor
is hidden

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

