###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetWindowData

Retrieve the data pointer associated with a window.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void* SDL_GetWindowData(SDL_Window * window,
                    const char *name);
```

## Function Parameters

|                            |            |                          |
| -------------------------- | ---------- | ------------------------ |
| [SDL_Window](SDL_Window) * | **window** | the window to query.     |
| const char *               | **name**   | the name of the pointer. |

## Return Value

(void *) Returns the value associated with `name`.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetWindowData](SDL_SetWindowData)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

