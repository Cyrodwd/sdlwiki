# SDL_CondWaitTimeout

Wait until a condition variable is signaled or a certain time has passed.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
int SDL_CondWaitTimeout(SDL_cond * cond,
                        SDL_mutex * mutex, Uint32 ms);
```

## Function Parameters

|                          |           |                                                                                                              |
| ------------------------ | --------- | ------------------------------------------------------------------------------------------------------------ |
| [SDL_cond](SDL_cond) *   | **cond**  | the condition variable to wait on.                                                                           |
| [SDL_mutex](SDL_mutex) * | **mutex** | the mutex used to coordinate thread access.                                                                  |
| [Uint32](Uint32)         | **ms**    | the maximum time to wait, in milliseconds, or [`SDL_MUTEX_MAXWAIT`](SDL_MUTEX_MAXWAIT) to wait indefinitely. |

## Return Value

(int) Returns 0 if the condition variable is signaled,
[`SDL_MUTEX_TIMEDOUT`](SDL_MUTEX_TIMEDOUT) if the condition is not signaled
in the allotted time, or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function unlocks the specified `mutex` and waits for another thread to
call [SDL_CondSignal](SDL_CondSignal)() or
[SDL_CondBroadcast](SDL_CondBroadcast)() on the condition variable `cond`,
or for the specified time to elapse. Once the condition variable is
signaled or the time elapsed, the mutex is re-locked and the function
returns.

The mutex must be locked before calling this function.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CondBroadcast](SDL_CondBroadcast)
- [SDL_CondSignal](SDL_CondSignal)
- [SDL_CondWait](SDL_CondWait)
- [SDL_CreateCond](SDL_CreateCond)
- [SDL_DestroyCond](SDL_DestroyCond)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

