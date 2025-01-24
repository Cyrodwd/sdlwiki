# SDL_SetRelativeMouseMode

Set relative mouse mode.

## Header File

Defined in [SDL_mouse.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mouse.h)

## Syntax

```c
int SDL_SetRelativeMouseMode(SDL_bool enabled);
```

## Function Parameters

|                      |             |                                                                                  |
| -------------------- | ----------- | -------------------------------------------------------------------------------- |
| [SDL_bool](SDL_bool) | **enabled** | [SDL_TRUE](SDL_TRUE) to enable relative mode, [SDL_FALSE](SDL_FALSE) to disable. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

If relative mode is not supported, this returns -1.

## Remarks

While the mouse is in relative mode, the cursor is hidden, the mouse
position is constrained to the window, and SDL will report continuous
relative mouse motion even if the mouse is at the edge of the window.

This function will flush any pending mouse motion.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetRelativeMouseMode](SDL_GetRelativeMouseMode)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMouse](CategoryMouse)

