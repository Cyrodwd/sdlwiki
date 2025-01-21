###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_DisableScreenSaver

Prevent the screen from being blanked by a screen saver.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_DisableScreenSaver(void);
```

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

If you disable the screensaver, it is automatically re-enabled when SDL
quits.

The screensaver is disabled by default, but this may by changed by
[SDL_HINT_VIDEO_ALLOW_SCREENSAVER](SDL_HINT_VIDEO_ALLOW_SCREENSAVER).

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_EnableScreenSaver](SDL_EnableScreenSaver)
- [SDL_ScreenSaverEnabled](SDL_ScreenSaverEnabled)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

