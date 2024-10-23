###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GL_GetAttribute

Get the actual value for an attribute from the current context.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GL_GetAttribute(SDL_GLattr attr, int *value);
```

## Function Parameters

|                          |           |                                                                                |
| ------------------------ | --------- | ------------------------------------------------------------------------------ |
| [SDL_GLattr](SDL_GLattr) | **attr**  | an [SDL_GLattr](SDL_GLattr) enum value specifying the OpenGL attribute to get. |
| int *                    | **value** | a pointer filled in with the current value of `attr`.                          |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_GL_ResetAttributes](SDL_GL_ResetAttributes)
- [SDL_GL_SetAttribute](SDL_GL_SetAttribute)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

