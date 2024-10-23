###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetDisplayForPoint

Get the display containing a point.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
SDL_DisplayID SDL_GetDisplayForPoint(const SDL_Point *point);
```

## Function Parameters

|                                |           |                     |
| ------------------------------ | --------- | ------------------- |
| const [SDL_Point](SDL_Point) * | **point** | the point to query. |

## Return Value

([SDL_DisplayID](SDL_DisplayID)) Returns the instance ID of the display
containing the point or 0 on failure; call [SDL_GetError](SDL_GetError)()
for more information.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_GetDisplayBounds](SDL_GetDisplayBounds)
- [SDL_GetDisplays](SDL_GetDisplays)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

