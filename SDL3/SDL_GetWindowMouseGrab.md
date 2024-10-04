###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetWindowMouseGrab

Get a window's mouse grab mode.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GetWindowMouseGrab(SDL_Window *window);
```

## Function Parameters

|                            |            |                      |
| -------------------------- | ---------- | -------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to query. |

## Return Value

(bool) Returns true if mouse is grabbed, and false otherwise.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_SetWindowKeyboardGrab](SDL_SetWindowKeyboardGrab)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

