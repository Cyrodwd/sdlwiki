###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_CreateTexture

Create a texture for a rendering context.

## Header File

Defined in [<SDL3/SDL_render.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_render.h)

## Syntax

```c
SDL_Texture * SDL_CreateTexture(SDL_Renderer *renderer, SDL_PixelFormat format, SDL_TextureAccess access, int w, int h);
```

## Function Parameters

|                                        |              |                                                                         |
| -------------------------------------- | ------------ | ----------------------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) *         | **renderer** | the rendering context.                                                  |
| [SDL_PixelFormat](SDL_PixelFormat)     | **format**   | one of the enumerated values in [SDL_PixelFormat](SDL_PixelFormat).     |
| [SDL_TextureAccess](SDL_TextureAccess) | **access**   | one of the enumerated values in [SDL_TextureAccess](SDL_TextureAccess). |
| int                                    | **w**        | the width of the texture in pixels.                                     |
| int                                    | **h**        | the height of the texture in pixels.                                    |

## Return Value

([SDL_Texture](SDL_Texture) *) Returns a pointer to the created texture or
NULL if no rendering context was active, the format was unsupported, or the
width or height were out of range; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

The contents of a texture when first created are not defined.

## Thread Safety

You may only call this function from the main thread.

## Version

This function is available since SDL 3.1.3.

## Code Examples

```c
#include <SDL3/SDL.h>

#include <stdlib.h>

/* Moving Rectangle */
int main(int argc, char *argv[])
{
        SDL_Window *window;
        SDL_Renderer *renderer;
        SDL_Texture *texture;
        SDL_Event event;
        SDL_FRect r;

        if (!SDL_Init(SDL_INIT_VIDEO)) {
                SDL_LogError(SDL_LOG_CATEGORY_APPLICATION, "Couldn't initialize SDL: %s", SDL_GetError());
                return 3;
        }

        window = SDL_CreateWindow("SDL_CreateTexture",
                        1024, 768,
                        SDL_WINDOW_RESIZABLE);

        r.w = 100;
        r.h = 50;

        renderer = SDL_CreateRenderer(window, NULL);

        texture = SDL_CreateTexture(renderer, SDL_PIXELFORMAT_RGBA8888, SDL_TEXTUREACCESS_TARGET, 1024, 768);

        while (1) {
                SDL_PollEvent(&event);
                if(event.type == SDL_EVENT_QUIT)
                        break;
                r.x=rand()%500;
                r.y=rand()%500;

                SDL_SetRenderTarget(renderer, texture);
                SDL_SetRenderDrawColor(renderer, 0x00, 0x00, 0x00, 0x00);
                SDL_RenderClear(renderer);
                SDL_RenderRect(renderer,&r);
                SDL_SetRenderDrawColor(renderer, 0xFF, 0x00, 0x00, 0x00);
                SDL_RenderFillRect(renderer, &r);
                SDL_SetRenderTarget(renderer, NULL);
                SDL_RenderTexture(renderer, texture, NULL, NULL);
                SDL_RenderPresent(renderer);
        }
        SDL_DestroyRenderer(renderer);
        SDL_Quit();
        return 0;
}

```

## See Also

- [SDL_CreateTextureFromSurface](SDL_CreateTextureFromSurface)
- [SDL_CreateTextureWithProperties](SDL_CreateTextureWithProperties)
- [SDL_DestroyTexture](SDL_DestroyTexture)
- [SDL_GetTextureSize](SDL_GetTextureSize)
- [SDL_UpdateTexture](SDL_UpdateTexture)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRender](CategoryRender)

