# SDL_GetShapedWindowMode

Get the shape parameters of a shaped window.

## Header File

Defined in [SDL_shape.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_shape.h)

## Syntax

```c
int SDL_GetShapedWindowMode(SDL_Window *window,SDL_WindowShapeMode *shape_mode);
```

## Function Parameters

|                                              |                |                                                                                         |
| -------------------------------------------- | -------------- | --------------------------------------------------------------------------------------- |
| [SDL_Window](SDL_Window) *                   | **window**     | The shaped window whose parameters should be retrieved.                                 |
| [SDL_WindowShapeMode](SDL_WindowShapeMode) * | **shape_mode** | An empty shape-mode structure to fill, or NULL to check whether the window has a shape. |

## Return Value

(int) Return 0 if the window has a shape and, provided shape_mode was not
NULL, shape_mode has been filled with the mode data,
[SDL_NONSHAPEABLE_WINDOW](SDL_NONSHAPEABLE_WINDOW) if the
[SDL_Window](SDL_Window) given is not a shaped window, or
[SDL_WINDOW_LACKS_SHAPE](SDL_WINDOW_LACKS_SHAPE) if the
[SDL_Window](SDL_Window) given is a shapeable window currently lacking a
shape.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_WindowShapeMode](SDL_WindowShapeMode)
- [SDL_SetWindowShape](SDL_SetWindowShape)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryShape](CategoryShape)

