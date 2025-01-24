# SDL_HINT_VIDEO_MAC_FULLSCREEN_SPACES

A variable that dictates policy for fullscreen Spaces on Mac OS X.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_VIDEO_MAC_FULLSCREEN_SPACES    "SDL_VIDEO_MAC_FULLSCREEN_SPACES"
```

## Remarks

This hint only applies to Mac OS X.

The variable can be set to the following values:

- "0": Disable Spaces support (FULLSCREEN_DESKTOP won't use them and
  [SDL_WINDOW_RESIZABLE](SDL_WINDOW_RESIZABLE) windows won't offer the
  "fullscreen" button on their titlebars).
- "1": Enable Spaces support (FULLSCREEN_DESKTOP will use them and
  [SDL_WINDOW_RESIZABLE](SDL_WINDOW_RESIZABLE) windows will offer the
  "fullscreen" button on their titlebars).

The default value is "1". This hint must be set before any windows are
created.





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

