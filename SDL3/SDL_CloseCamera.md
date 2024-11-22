###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_CloseCamera

Use this function to shut down camera processing and close the camera device.

## Header File

Defined in [<SDL3/SDL_camera.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_camera.h)

## Syntax

```c
void SDL_CloseCamera(SDL_Camera *camera);
```

## Function Parameters

|                            |            |                       |
| -------------------------- | ---------- | --------------------- |
| [SDL_Camera](SDL_Camera) * | **camera** | opened camera device. |

## Thread Safety

It is safe to call this function from any thread, but no thread may
reference `device` once this function is called.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_OpenCamera](SDL_OpenCamera)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryCamera](CategoryCamera)

