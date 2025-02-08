# SDL_GetCurrentVideoDriver

Get the name of the currently initialized video driver.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
const char* SDL_GetCurrentVideoDriver(void);
```

## Return Value

(const char *) Returns the name of the current video driver or NULL if no
driver has been initialized.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetNumVideoDrivers](SDL_GetNumVideoDrivers)
- [SDL_GetVideoDriver](SDL_GetVideoDriver)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

