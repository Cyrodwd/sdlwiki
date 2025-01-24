# SDL_GetWindowMaximumSize

Get the maximum size of a window's client area.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GetWindowMaximumSize(SDL_Window *window, int *w, int *h);
```

## Function Parameters

|                            |            |                                                                         |
| -------------------------- | ---------- | ----------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to query.                                                    |
| int *                      | **w**      | a pointer filled in with the maximum width of the window, may be NULL.  |
| int *                      | **h**      | a pointer filled in with the maximum height of the window, may be NULL. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetWindowMinimumSize](SDL_GetWindowMinimumSize)
- [SDL_SetWindowMaximumSize](SDL_SetWindowMaximumSize)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

