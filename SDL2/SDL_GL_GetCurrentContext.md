# SDL_GL_GetCurrentContext

Get the currently active OpenGL context.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
SDL_GLContext SDL_GL_GetCurrentContext(void);
```

## Return Value

([SDL_GLContext](SDL_GLContext)) Returns the currently active OpenGL
context or NULL on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GL_MakeCurrent](SDL_GL_MakeCurrent)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

