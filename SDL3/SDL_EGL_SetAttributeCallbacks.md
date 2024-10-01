###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_EGL_SetAttributeCallbacks

Sets the callbacks for defining custom EGLAttrib arrays for EGL initialization.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
void SDL_EGL_SetAttributeCallbacks(SDL_EGLAttribArrayCallback platformAttribCallback,
                                  SDL_EGLIntArrayCallback surfaceAttribCallback,
                                  SDL_EGLIntArrayCallback contextAttribCallback, void *userdata);
```

## Function Parameters

|                                                          |                            |                                                           |
| -------------------------------------------------------- | -------------------------- | --------------------------------------------------------- |
| [SDL_EGLAttribArrayCallback](SDL_EGLAttribArrayCallback) | **platformAttribCallback** | callback for attributes to pass to eglGetPlatformDisplay. |
| [SDL_EGLIntArrayCallback](SDL_EGLIntArrayCallback)       | **surfaceAttribCallback**  | callback for attributes to pass to eglCreateSurface.      |
| [SDL_EGLIntArrayCallback](SDL_EGLIntArrayCallback)       | **contextAttribCallback**  | callback for attributes to pass to eglCreateContext.      |
| void *                                                   | **userdata**               | a pointer that is passed to the callbacks.                |

## Remarks

Each callback should return a pointer to an EGL attribute array terminated
with EGL_NONE. Callbacks may return NULL pointers to signal an error, which
will cause the [SDL_CreateWindow](SDL_CreateWindow) process to fail
gracefully.

The arrays returned by each callback will be appended to the existing
attribute arrays defined by SDL.

NOTE: These callback pointers will be reset after
[SDL_GL_ResetAttributes](SDL_GL_ResetAttributes).

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

