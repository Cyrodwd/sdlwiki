###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GL_SwapWindow

Update a window with OpenGL rendering.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
bool SDL_GL_SwapWindow(SDL_Window *window);
```

## Function Parameters

|                            |            |                       |
| -------------------------- | ---------- | --------------------- |
| [SDL_Window](SDL_Window) * | **window** | the window to change. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This is used with double-buffered OpenGL contexts, which are the default.

On macOS, make sure you bind 0 to the draw framebuffer before swapping the
window, otherwise nothing will happen. If you aren't using
glBindFramebuffer(), this is the default and you won't have to do anything
extra.

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.1.3.

## Code Examples

```c

SDL_Window* window = SDL_CreateWindow("SDL3/OpenGL Demo", 640, 480, SDL_WINDOW_OPENGL|SDL_WINDOW_RESIZABLE);
      
/* Create an OpenGL context associated with the window. */
SDL_GLContext glcontext = SDL_GL_CreateContext(window);

/* This makes our buffer swap syncronized with the monitor's vertical refresh */
SDL_GL_SetSwapInterval(1);

/* Clear context */
glClearColor(0,0,0,1);
glClear(GL_COLOR_BUFFER_BIT);

/* <Extra drawing functions here> */ 

/* Swap our buffer to display the current contents of buffer on screen */ 
SDL_GL_SwapWindow(window);


```

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

