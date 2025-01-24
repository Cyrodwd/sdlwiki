# SDL_SetAtomicInt

Set an atomic variable to a value.

## Header File

Defined in [<SDL3/SDL_atomic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_atomic.h)

## Syntax

```c
int SDL_SetAtomicInt(SDL_AtomicInt *a, int v);
```

## Function Parameters

|                                  |       |                                                                         |
| -------------------------------- | ----- | ----------------------------------------------------------------------- |
| [SDL_AtomicInt](SDL_AtomicInt) * | **a** | a pointer to an [SDL_AtomicInt](SDL_AtomicInt) variable to be modified. |
| int                              | **v** | the desired value.                                                      |

## Return Value

(int) Returns the previous value of the atomic variable.

## Remarks

This function also acts as a full memory barrier.

***Note: If you don't know what this function is for, you shouldn't use
it!***

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetAtomicInt](SDL_GetAtomicInt)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAtomic](CategoryAtomic)

