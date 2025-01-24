# SDL_DisableScreenSaver

Prevent the screen from being blanked by a screen saver.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
void SDL_DisableScreenSaver(void);
```

## Remarks

If you disable the screensaver, it is automatically re-enabled when SDL
quits.

The screensaver is disabled by default since SDL 2.0.2. Before SDL 2.0.2
the screensaver was enabled by default.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_EnableScreenSaver](SDL_EnableScreenSaver)
- [SDL_IsScreenSaverEnabled](SDL_IsScreenSaverEnabled)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

