###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_AtomicDecRef

Decrement an atomic variable used as a reference count.

## Header File

Defined in [<SDL3/SDL_atomic.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_atomic.h)

## Syntax

```c
#define SDL_AtomicDecRef(a)    (SDL_AddAtomicInt(a, -1) == 1)
```

## Macro Parameters

|       |                                                              |
| ----- | ------------------------------------------------------------ |
| **a** | a pointer to an [SDL_AtomicInt](SDL_AtomicInt) to increment. |

## Return Value

Returns true if the variable reached zero after decrementing, false
otherwise.

## Remarks

***Note: If you don't know what this macro is for, you shouldn't use it!***

## Version

This macro is available since SDL 3.0.0.

## See Also

- [SDL_AtomicIncRef](SDL_AtomicIncRef)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryAtomic](CategoryAtomic)

