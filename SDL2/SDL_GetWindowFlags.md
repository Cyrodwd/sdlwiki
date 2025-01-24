# SDL_GetWindowFlags

Get the window flags.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
Uint32 SDL_GetWindowFlags(SDL_Window * window);
```

## Function Parameters

|                            |            |                      |
| -------------------------- | ---------- | -------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to query. |

## Return Value

([Uint32](Uint32)) Returns a mask of the [SDL_WindowFlags](SDL_WindowFlags)
associated with `window`.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateWindow](SDL_CreateWindow)
- [SDL_HideWindow](SDL_HideWindow)
- [SDL_MaximizeWindow](SDL_MaximizeWindow)
- [SDL_MinimizeWindow](SDL_MinimizeWindow)
- [SDL_SetWindowFullscreen](SDL_SetWindowFullscreen)
- [SDL_SetWindowGrab](SDL_SetWindowGrab)
- [SDL_ShowWindow](SDL_ShowWindow)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

