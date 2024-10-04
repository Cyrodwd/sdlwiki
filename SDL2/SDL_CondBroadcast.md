###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_CondBroadcast

Restart all threads that are waiting on the condition variable.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
int SDL_CondBroadcast(SDL_cond * cond);
```

## Function Parameters

|                        |          |                                   |
| ---------------------- | -------- | --------------------------------- |
| [SDL_cond](SDL_cond) * | **cond** | the condition variable to signal. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CondSignal](SDL_CondSignal)
- [SDL_CondWait](SDL_CondWait)
- [SDL_CondWaitTimeout](SDL_CondWaitTimeout)
- [SDL_CreateCond](SDL_CreateCond)
- [SDL_DestroyCond](SDL_DestroyCond)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

