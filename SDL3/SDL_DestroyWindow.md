###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_DestroyWindow

Destroy a window.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
void SDL_DestroyWindow(SDL_Window *window);
```

## Function Parameters

|                            |            |                        |
| -------------------------- | ---------- | ---------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to destroy. |

## Remarks

Any popups or modal windows owned by the window will be recursively
destroyed as well.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_CreatePopupWindow](SDL_CreatePopupWindow)
- [SDL_CreateWindow](SDL_CreateWindow)
- [SDL_CreateWindowWithProperties](SDL_CreateWindowWithProperties)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

