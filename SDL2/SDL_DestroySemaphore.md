###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_DestroySemaphore

Destroy a semaphore.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
void SDL_DestroySemaphore(SDL_sem * sem);
```

## Function Parameters

|                      |         |                           |
| -------------------- | ------- | ------------------------- |
| [SDL_sem](SDL_sem) * | **sem** | the semaphore to destroy. |

## Remarks

It is not safe to destroy a semaphore if there are threads currently
waiting on it.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateSemaphore](SDL_CreateSemaphore)
- [SDL_SemPost](SDL_SemPost)
- [SDL_SemTryWait](SDL_SemTryWait)
- [SDL_SemValue](SDL_SemValue)
- [SDL_SemWait](SDL_SemWait)
- [SDL_SemWaitTimeout](SDL_SemWaitTimeout)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

