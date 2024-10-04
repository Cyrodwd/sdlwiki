###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_UnlockMutex

Unlock the mutex.

## Header File

Defined in [SDL_mutex.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mutex.h)

## Syntax

```c
int SDL_UnlockMutex(SDL_mutex * mutex);

#define SDL_mutexV(m)   SDL_UnlockMutex(m)
```

## Function Parameters

|                          |           |                      |
| ------------------------ | --------- | -------------------- |
| [SDL_mutex](SDL_mutex) * | **mutex** | the mutex to unlock. |

## Return Value

(int) Returns 0, or -1 on error.

## Remarks

It is legal for the owning thread to lock an already-locked mutex. It must
unlock it the same number of times before it is actually made available for
other threads in the system (this is known as a "recursive mutex").

It is an error to unlock a mutex that has not been locked by the current
thread, and doing so results in undefined behavior.

It is also an error to unlock a mutex that isn't locked at all.

## Version

This function is available since SDL 2.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMutex](CategoryMutex)

