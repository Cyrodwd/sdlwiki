###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_LogGetOutputFunction

Get the current log output function.

## Header File

Defined in [SDL_log.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_log.h)

## Syntax

```c
void SDL_LogGetOutputFunction(SDL_LogOutputFunction *callback, void **userdata);
```

## Function Parameters

|                                                  |              |                                                                                            |
| ------------------------------------------------ | ------------ | ------------------------------------------------------------------------------------------ |
| [SDL_LogOutputFunction](SDL_LogOutputFunction) * | **callback** | an [SDL_LogOutputFunction](SDL_LogOutputFunction) filled in with the current log callback. |
| void **                                          | **userdata** | a pointer filled in with the pointer that is passed to `callback`.                         |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_LogSetOutputFunction](SDL_LogSetOutputFunction)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLog](CategoryLog)

