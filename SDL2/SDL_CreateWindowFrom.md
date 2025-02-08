# SDL_CreateWindowFrom

Create an SDL window from an existing native window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
SDL_Window * SDL_CreateWindowFrom(const void *data);
```

## Function Parameters

|              |          |                                                                                                   |
| ------------ | -------- | ------------------------------------------------------------------------------------------------- |
| const void * | **data** | a pointer to driver-dependent window creation data, typically your native window cast to a void*. |

## Return Value

([SDL_Window](SDL_Window) *) Returns the window that was created or NULL on
failure; call [SDL_GetError](SDL_GetError)() for more information.

## Remarks

In some cases (e.g. OpenGL) and on some platforms (e.g. Microsoft Windows)
the hint
[`SDL_HINT_VIDEO_WINDOW_SHARE_PIXEL_FORMAT`](SDL_HINT_VIDEO_WINDOW_SHARE_PIXEL_FORMAT)
needs to be configured before using
[SDL_CreateWindowFrom](SDL_CreateWindowFrom)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateWindow](SDL_CreateWindow)
- [SDL_DestroyWindow](SDL_DestroyWindow)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

