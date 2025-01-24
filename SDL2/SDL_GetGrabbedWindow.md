# SDL_GetGrabbedWindow

Get the window that currently has an input grab enabled.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
SDL_Window * SDL_GetGrabbedWindow(void);
```

## Return Value

([SDL_Window](SDL_Window) *) Returns the window if input is grabbed or NULL
otherwise.

## Version

This function is available since SDL 2.0.4.

## See Also

- [SDL_GetWindowGrab](SDL_GetWindowGrab)
- [SDL_SetWindowGrab](SDL_SetWindowGrab)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

