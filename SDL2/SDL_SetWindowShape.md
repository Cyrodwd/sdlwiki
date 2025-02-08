# SDL_SetWindowShape

Set the shape and parameters of a shaped window.

## Header File

Defined in [SDL_shape.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_shape.h)

## Syntax

```c
int SDL_SetWindowShape(SDL_Window *window,SDL_Surface *shape,SDL_WindowShapeMode *shape_mode);
```

## Function Parameters

|                                              |                |                                                      |
| -------------------------------------------- | -------------- | ---------------------------------------------------- |
| [SDL_Window](SDL_Window) *                   | **window**     | The shaped window whose parameters should be set.    |
| [SDL_Surface](SDL_Surface) *                 | **shape**      | A surface encoding the desired shape for the window. |
| [SDL_WindowShapeMode](SDL_WindowShapeMode) * | **shape_mode** | The parameters to set for the shaped window.         |

## Return Value

(int) Return 0 on success,
[SDL_INVALID_SHAPE_ARGUMENT](SDL_INVALID_SHAPE_ARGUMENT) on an invalid
shape argument, or [SDL_NONSHAPEABLE_WINDOW](SDL_NONSHAPEABLE_WINDOW) if
the [SDL_Window](SDL_Window) given does not reference a valid shaped
window.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_WindowShapeMode](SDL_WindowShapeMode)
- [SDL_GetShapedWindowMode](SDL_GetShapedWindowMode)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryShape](CategoryShape)

