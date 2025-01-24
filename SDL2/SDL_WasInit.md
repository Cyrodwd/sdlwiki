# SDL_WasInit

Get a mask of the specified subsystems which are currently initialized.

## Header File

Defined in [SDL.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL.h)

## Syntax

```c
Uint32 SDL_WasInit(Uint32 flags);
```

## Function Parameters

|                  |           |                                                                                        |
| ---------------- | --------- | -------------------------------------------------------------------------------------- |
| [Uint32](Uint32) | **flags** | any of the flags used by [SDL_Init](SDL_Init)(); see [SDL_Init](SDL_Init) for details. |

## Return Value

([Uint32](Uint32)) Returns a mask of all initialized subsystems if `flags`
is 0, otherwise it returns the initialization status of the specified
subsystems.

The return value does not include
[SDL_INIT_NOPARACHUTE](SDL_INIT_NOPARACHUTE).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_Init](SDL_Init)
- [SDL_InitSubSystem](SDL_InitSubSystem)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryInit](CategoryInit)

