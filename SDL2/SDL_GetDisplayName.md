# SDL_GetDisplayName

Get the name of a display in UTF-8 encoding.

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
const char * SDL_GetDisplayName(int displayIndex);
```

## Function Parameters

|     |                  |                                                             |
| --- | ---------------- | ----------------------------------------------------------- |
| int | **displayIndex** | the index of display from which the name should be queried. |

## Return Value

(const char *) Returns the name of a display or NULL for an invalid display
index or failure; call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetNumVideoDisplays](SDL_GetNumVideoDisplays)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVideo](CategoryVideo)

