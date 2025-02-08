# SDL_GL_SetAttribute

Set an OpenGL window attribute before window creation.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_GL_SetAttribute(SDL_GLattr attr, int value);
```

## Function Parameters

|                          |           |                                                                                |
| ------------------------ | --------- | ------------------------------------------------------------------------------ |
| [SDL_GLattr](SDL_GLattr) | **attr**  | an [SDL_GLattr](SDL_GLattr) enum value specifying the OpenGL attribute to set. |
| int                      | **value** | the desired value for the attribute.                                           |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function sets the OpenGL attribute `attr` to `value`. The requested
attributes should be set before creating an OpenGL window. You should use
[SDL_GL_GetAttribute](SDL_GL_GetAttribute)() to check the values after
creating the OpenGL context, since the values obtained can differ from the
requested ones.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GL_GetAttribute](SDL_GL_GetAttribute)
- [SDL_GL_ResetAttributes](SDL_GL_ResetAttributes)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

