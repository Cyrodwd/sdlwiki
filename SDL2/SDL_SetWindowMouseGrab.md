# SDL_SetWindowMouseGrab

Set a window's mouse grab mode.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void SDL_SetWindowMouseGrab(SDL_Window * window,
                            SDL_bool grabbed);
```

## Function Parameters

|                            |             |                                                                                    |
| -------------------------- | ----------- | ---------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) * | **window**  | The window for which the mouse grab mode should be set.                            |
| [SDL_bool](SDL_bool)       | **grabbed** | This is [SDL_TRUE](SDL_TRUE) to grab mouse, and [SDL_FALSE](SDL_FALSE) to release. |

## Remarks

Mouse grab confines the mouse cursor to the window.

## Version

This function is available since SDL 2.0.16.

## See Also

- [SDL_GetWindowMouseGrab](SDL_GetWindowMouseGrab)
- [SDL_SetWindowKeyboardGrab](SDL_SetWindowKeyboardGrab)
- [SDL_SetWindowGrab](SDL_SetWindowGrab)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

