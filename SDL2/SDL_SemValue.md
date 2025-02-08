# SDL_SemValue

Get the current value of a semaphore.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
Uint32 SDL_SemValue(SDL_sem * sem);
```

## Function Parameters

|                      |         |                         |
| -------------------- | ------- | ----------------------- |
| [SDL_sem](SDL_sem) * | **sem** | the semaphore to query. |

## Return Value

([Uint32](Uint32)) Returns the current value of the semaphore.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateSemaphore](SDL_CreateSemaphore)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

