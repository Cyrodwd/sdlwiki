###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_AtomicTryLock

Try to lock a spin lock by setting it to a non-zero value.

## Header File

Defined in [SDL_atomic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_atomic.h)

## Syntax

```c
SDL_bool SDL_AtomicTryLock(SDL_SpinLock *lock);
```

## Function Parameters

|                                |          |                               |
| ------------------------------ | -------- | ----------------------------- |
| [SDL_SpinLock](SDL_SpinLock) * | **lock** | a pointer to a lock variable. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if the lock succeeded,
[SDL_FALSE](SDL_FALSE) if the lock is already held.

## Remarks

***Please note that spinlocks are dangerous if you don't know what you're
doing. Please be careful using any sort of spinlock!***

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_AtomicLock](SDL_AtomicLock)
- [SDL_AtomicUnlock](SDL_AtomicUnlock)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAtomic](CategoryAtomic)

