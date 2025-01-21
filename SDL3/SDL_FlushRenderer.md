###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_FlushRenderer

Force the rendering context to flush any pending commands and state.

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
bool SDL_FlushRenderer(SDL_Renderer *renderer);
```

## Function Parameters

|                                |              |                        |
| ------------------------------ | ------------ | ---------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

You do not need to (and in fact, shouldn't) call this function unless you
are planning to call into OpenGL/Direct3D/Metal/whatever directly, in
addition to using an [SDL_Renderer](SDL_Renderer).

This is for a very-specific case: if you are using SDL's render API, and
you plan to make OpenGL/D3D/whatever calls in addition to SDL render API
calls. If this applies, you should call this function between calls to
SDL's render API and the low-level API you're using in cooperation.

In all other cases, you can ignore this function.

This call makes SDL flush any pending rendering work it was queueing up to
do later in a single batch, and marks any internal cached state as invalid,
so it'll prepare all its state again later, from scratch.

This means you do not need to save state in your rendering code to protect
the SDL renderer. However, there lots of arbitrary pieces of Direct3D and
OpenGL state that can confuse things; you should use your best judgment and
be prepared to make changes if specific state needs to be protected.

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

