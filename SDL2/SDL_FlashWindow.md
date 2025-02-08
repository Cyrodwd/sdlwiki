# SDL_FlashWindow

Request a window to demand attention from the user.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_FlashWindow(SDL_Window * window, SDL_FlashOperation operation);
```

## Function Parameters

|                                          |               |                           |
| ---------------------------------------- | ------------- | ------------------------- |
| [SDL_Window](SDL_Window) *               | **window**    | the window to be flashed. |
| [SDL_FlashOperation](SDL_FlashOperation) | **operation** | the flash operation.      |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.16.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

