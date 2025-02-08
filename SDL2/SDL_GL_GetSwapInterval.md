# SDL_GL_GetSwapInterval

Get the swap interval for the current OpenGL context.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_GL_GetSwapInterval(void);
```

## Return Value

(int) Returns 0 if there is no vertical retrace synchronization, 1 if the
buffer swap is synchronized with the vertical retrace, and -1 if late swaps
happen immediately instead of waiting for the next retrace; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

If the system can't determine the swap interval, or there isn't a valid
current context, this function will return 0 as a safe default.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GL_SetSwapInterval](SDL_GL_SetSwapInterval)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

