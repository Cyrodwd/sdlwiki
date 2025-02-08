# SDL_GetWindowFromID

Get a window from a stored ID.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
SDL_Window * SDL_GetWindowFromID(Uint32 id);
```

## Function Parameters

|                  |        |                       |
| ---------------- | ------ | --------------------- |
| [Uint32](Uint32) | **id** | the ID of the window. |

## Return Value

([SDL_Window](SDL_Window) *) Returns the window associated with `id` or
NULL if it doesn't exist; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

The numeric ID is what [SDL_WindowEvent](SDL_WindowEvent) references, and
is necessary to map these events to specific [SDL_Window](SDL_Window)
objects.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetWindowID](SDL_GetWindowID)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

