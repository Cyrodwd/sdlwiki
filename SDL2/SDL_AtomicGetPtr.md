# SDL_AtomicGetPtr

Get the value of a pointer atomically.

## Header File

Defined in [SDL_atomic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_atomic.h)

## Syntax

```c
void* SDL_AtomicGetPtr(void **a);
```

## Function Parameters

|         |       |                         |
| ------- | ----- | ----------------------- |
| void ** | **a** | a pointer to a pointer. |

## Return Value

(void *) Returns the current value of a pointer.

## Remarks

***Note: If you don't know what this function is for, you shouldn't use
it!***

## Version

This function is available since SDL 2.0.2.

## See Also

- [SDL_AtomicCASPtr](SDL_AtomicCASPtr)
- [SDL_AtomicSetPtr](SDL_AtomicSetPtr)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAtomic](CategoryAtomic)

