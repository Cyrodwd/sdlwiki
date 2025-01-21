###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_UnlockMutex

Unlock the mutex.

## Header File

Defined in [<SDL3/SDL_mutex.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mutex.h)

## Syntax

```c
void SDL_UnlockMutex(SDL_Mutex *mutex);
```

## Function Parameters

|                          |           |                      |
| ------------------------ | --------- | -------------------- |
| [SDL_Mutex](SDL_Mutex) * | **mutex** | the mutex to unlock. |

## Remarks

It is legal for the owning thread to lock an already-locked mutex. It must
unlock it the same number of times before it is actually made available for
other threads in the system (this is known as a "recursive mutex").

It is illegal to unlock a mutex that has not been locked by the current
thread, and doing so results in undefined behavior.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_LockMutex](SDL_LockMutex)
- [SDL_TryLockMutex](SDL_TryLockMutex)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

