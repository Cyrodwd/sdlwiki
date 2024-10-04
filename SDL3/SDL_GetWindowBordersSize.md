###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetWindowBordersSize

Get the size of a window's borders (decorations) around the client area.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GetWindowBordersSize(SDL_Window *window, int *top, int *left, int *bottom, int *right);
```

## Function Parameters

|                            |            |                                                                                   |
| -------------------------- | ---------- | --------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to query the size values of the border (decorations) from.             |
| int *                      | **top**    | pointer to variable for storing the size of the top border; NULL is permitted.    |
| int *                      | **left**   | pointer to variable for storing the size of the left border; NULL is permitted.   |
| int *                      | **bottom** | pointer to variable for storing the size of the bottom border; NULL is permitted. |
| int *                      | **right**  | pointer to variable for storing the size of the right border; NULL is permitted.  |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Note: If this function fails (returns false), the size values will be
initialized to 0, 0, 0, 0 (if a non-NULL pointer is provided), as if the
window in question was borderless.

Note: This function may fail on systems where the window has not yet been
decorated by the display server (for example, immediately after calling
[SDL_CreateWindow](SDL_CreateWindow)). It is recommended that you wait at
least until the window has been presented and composited, so that the
window system has a chance to decorate the window and provide the border
dimensions to SDL.

This function also returns false if getting the information is not
supported.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetWindowSize](SDL_GetWindowSize)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

