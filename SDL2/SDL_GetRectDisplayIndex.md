# SDL_GetRectDisplayIndex

Get the index of the display primarily containing a rect

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
int SDL_GetRectDisplayIndex(const SDL_Rect * rect);
```

## Function Parameters

|                              |          |                    |
| ---------------------------- | -------- | ------------------ |
| const [SDL_Rect](SDL_Rect) * | **rect** | the rect to query. |

## Return Value

(int) Returns the index of the display entirely containing the rect or
closest to the center of the rect on success or a negative error code on
failure; call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.24.0.

## See Also

- [SDL_GetDisplayBounds](SDL_GetDisplayBounds)
- [SDL_GetNumVideoDisplays](SDL_GetNumVideoDisplays)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

