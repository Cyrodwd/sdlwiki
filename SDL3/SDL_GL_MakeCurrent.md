###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GL_MakeCurrent

Set up an OpenGL context for rendering into an OpenGL window.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GL_MakeCurrent(SDL_Window *window, SDL_GLContext context);
```

## Function Parameters

|                                |             |                                                  |
| ------------------------------ | ----------- | ------------------------------------------------ |
| [SDL_Window](SDL_Window) *     | **window**  | the window to associate with the context.        |
| [SDL_GLContext](SDL_GLContext) | **context** | the OpenGL context to associate with the window. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The context must have been created with a compatible window.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GL_CreateContext](SDL_GL_CreateContext)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

