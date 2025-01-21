###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_HINT_QUIT_ON_LAST_WINDOW_CLOSE

A variable that decides whether to send [SDL_EVENT_QUIT](SDL_EVENT_QUIT) when closing the last window.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_QUIT_ON_LAST_WINDOW_CLOSE "SDL_QUIT_ON_LAST_WINDOW_CLOSE"
```

## Remarks

The variable can be set to the following values:

- "0": SDL will not send an [SDL_EVENT_QUIT](SDL_EVENT_QUIT) event when the
  last window is requesting to close. Note that in this case, there are
  still other legitimate reasons one might get an
  [SDL_EVENT_QUIT](SDL_EVENT_QUIT) event: choosing "Quit" from the macOS
  menu bar, sending a SIGINT (ctrl-c) on Unix, etc.
- "1": SDL will send a quit event when the last window is requesting to
  close. (default)

If there is at least one active system tray icon,
[SDL_EVENT_QUIT](SDL_EVENT_QUIT) will instead be sent when both the last
window will be closed and the last tray icon will be destroyed.

This hint can be set anytime.

## Version

This hint is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

