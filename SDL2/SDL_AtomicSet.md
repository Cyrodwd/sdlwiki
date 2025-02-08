# SDL_AtomicSet

Set an atomic variable to a value.

## Header File

Defined in [SDL_atomic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_atomic.h)

## Syntax

```c
int SDL_AtomicSet(SDL_atomic_t *a, int v);
```

## Function Parameters

|                                |       |                                                                       |
| ------------------------------ | ----- | --------------------------------------------------------------------- |
| [SDL_atomic_t](SDL_atomic_t) * | **a** | a pointer to an [SDL_atomic_t](SDL_atomic_t) variable to be modified. |
| int                            | **v** | the desired value.                                                    |

## Return Value

(int) Returns the previous value of the atomic variable.

## Remarks

This function also acts as a full memory barrier.

***Note: If you don't know what this function is for, you shouldn't use
it!***

## Version

This function is available since SDL 2.0.2.

## See Also

- [SDL_AtomicGet](SDL_AtomicGet)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAtomic](CategoryAtomic)

