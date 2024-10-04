###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_RenderClear

Clear the current rendering target with the drawing color.

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
bool SDL_RenderClear(SDL_Renderer *renderer);
```

## Function Parameters

|                                |              |                        |
| ------------------------------ | ------------ | ---------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the rendering context. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function clears the entire rendering target, ignoring the viewport and
the clip rectangle. Note, that clearing will also set/fill all pixels of
the rendering target to current renderer draw color, so make sure to invoke
[SDL_SetRenderDrawColor](SDL_SetRenderDrawColor)() when needed.

## Thread Safety

You may only call this function from the main thread.

## Version

This function is available since SDL 3.0.0.

## Code Examples

```c
#include <SDL3/SDL.h>

int main(int argc, char* argv[])
{
        SDL_Window* window;
        SDL_Renderer* renderer;

        /* Initialize SDL. */
        if (!SDL_Init(SDL_INIT_VIDEO))
                return 1;

        /* Create the window where we will draw. */
        window = SDL_CreateWindow("SDL_RenderClear",
                        512, 512,
                        0);

        /* We must call SDL_CreateRenderer in order for draw calls to affect this window. */
        renderer = SDL_CreateRenderer(window, NULL);

        /* Select the color for drawing. It is set to red here. */
        SDL_SetRenderDrawColor(renderer, 255, 0, 0, 255);

        /* Clear the entire screen to our selected color. */
        SDL_RenderClear(renderer);

        /* Up until now everything was drawn behind the scenes.
           This will show the new, red contents of the window. */
        SDL_RenderPresent(renderer);

        /* Give us time to see the window. */
        SDL_Delay(5000);

        /* Always be sure to clean up */
        SDL_Quit();
        return 0;
}
```

## See Also

- [SDL_SetRenderDrawColor](SDL_SetRenderDrawColor)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

