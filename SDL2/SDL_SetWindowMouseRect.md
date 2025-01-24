# SDL_SetWindowMouseRect

Confines the cursor to the specified area of a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_SetWindowMouseRect(SDL_Window * window, const SDL_Rect * rect);
```

## Function Parameters

|                              |            |                                                                                                                  |
| ---------------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) *   | **window** | The window that will be associated with the barrier.                                                             |
| const [SDL_Rect](SDL_Rect) * | **rect**   | A rectangle area in window-relative coordinates. If NULL the barrier for the specified window will be destroyed. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Note that this does NOT grab the cursor, it only defines the area a cursor
is restricted to when the window has mouse focus.

## Version

This function is available since SDL 2.0.18.

## See Also

- [SDL_GetWindowMouseRect](SDL_GetWindowMouseRect)
- [SDL_SetWindowMouseGrab](SDL_SetWindowMouseGrab)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

