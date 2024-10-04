###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_AtomicSetPtr

Set a pointer to a value atomically.

## Header File

Defined in [SDL_atomic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_atomic.h)

## Syntax

```c
void* SDL_AtomicSetPtr(void **a, void* v);
```

## Function Parameters

|         |       |                            |
| ------- | ----- | -------------------------- |
| void ** | **a** | a pointer to a pointer.    |
| void *  | **v** | the desired pointer value. |

## Return Value

(void *) Returns the previous value of the pointer.

## Remarks

***Note: If you don't know what this function is for, you shouldn't use
it!***

## Version

This function is available since SDL 2.0.2.

## See Also

- [SDL_AtomicCASPtr](SDL_AtomicCASPtr)
- [SDL_AtomicGetPtr](SDL_AtomicGetPtr)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAtomic](CategoryAtomic)

