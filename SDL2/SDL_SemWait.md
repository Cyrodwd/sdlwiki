# SDL_SemWait

Wait until a semaphore has a positive value and then decrements it.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
int SDL_SemWait(SDL_sem * sem);
```

## Function Parameters

|                      |         |                        |
| -------------------- | ------- | ---------------------- |
| [SDL_sem](SDL_sem) * | **sem** | the semaphore wait on. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function suspends the calling thread until either the semaphore
pointed to by `sem` has a positive value or the call is interrupted by a
signal or error. If the call is successful it will atomically decrement the
semaphore value.

This function is the equivalent of calling
[SDL_SemWaitTimeout](SDL_SemWaitTimeout)() with a time length of
[`SDL_MUTEX_MAXWAIT`](SDL_MUTEX_MAXWAIT).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateSemaphore](SDL_CreateSemaphore)
- [SDL_DestroySemaphore](SDL_DestroySemaphore)
- [SDL_SemPost](SDL_SemPost)
- [SDL_SemTryWait](SDL_SemTryWait)
- [SDL_SemValue](SDL_SemValue)
- [SDL_SemWait](SDL_SemWait)
- [SDL_SemWaitTimeout](SDL_SemWaitTimeout)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

