###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_InitSubSystem

Compatibility function to initialize the SDL library.

## Header File

Defined in [SDL.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL.h)

## Syntax

```c
int SDL_InitSubSystem(Uint32 flags);
```

## Function Parameters

|                  |           |                                                                                        |
| ---------------- | --------- | -------------------------------------------------------------------------------------- |
| [Uint32](Uint32) | **flags** | any of the flags used by [SDL_Init](SDL_Init)(); see [SDL_Init](SDL_Init) for details. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

In SDL2, this function and [SDL_Init](SDL_Init)() are interchangeable.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_Init](SDL_Init)
- [SDL_Quit](SDL_Quit)
- [SDL_QuitSubSystem](SDL_QuitSubSystem)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryInit](CategoryInit)

