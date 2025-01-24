# SDL_GetWindowSize

Get the size of a window's client area.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GetWindowSize(SDL_Window *window, int *w, int *h);
```

## Function Parameters

|                            |            |                                                                 |
| -------------------------- | ---------- | --------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to query the width and height from.                  |
| int *                      | **w**      | a pointer filled in with the width of the window, may be NULL.  |
| int *                      | **h**      | a pointer filled in with the height of the window, may be NULL. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The window pixel size may differ from its window coordinate size if the
window is on a high pixel density display. Use
[SDL_GetWindowSizeInPixels](SDL_GetWindowSizeInPixels)() or
[SDL_GetRenderOutputSize](SDL_GetRenderOutputSize)() to get the real client
area size in pixels.

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetRenderOutputSize](SDL_GetRenderOutputSize)
- [SDL_GetWindowSizeInPixels](SDL_GetWindowSizeInPixels)
- [SDL_SetWindowSize](SDL_SetWindowSize)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

