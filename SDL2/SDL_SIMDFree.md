###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SIMDFree

Deallocate memory obtained from [SDL_SIMDAlloc](SDL_SIMDAlloc)

## Header File

Defined in [SDL_cpuinfo.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_cpuinfo.h)

## Syntax

```c
void SDL_SIMDFree(void *ptr);
```

## Function Parameters

|        |         |                                                                                                                                        |
| ------ | ------- | -------------------------------------------------------------------------------------------------------------------------------------- |
| void * | **ptr** | The pointer, returned from [SDL_SIMDAlloc](SDL_SIMDAlloc) or [SDL_SIMDRealloc](SDL_SIMDRealloc), to deallocate. NULL is a legal no-op. |

## Remarks

It is not valid to use this function on a pointer from anything but
[SDL_SIMDAlloc](SDL_SIMDAlloc)() or [SDL_SIMDRealloc](SDL_SIMDRealloc)().
It can't be used on pointers from malloc, realloc,
[SDL_malloc](SDL_malloc), memalign, new[], etc.

However, [SDL_SIMDFree](SDL_SIMDFree)(NULL) is a legal no-op.

The memory pointed to by `ptr` is no longer valid for access upon return,
and may be returned to the system or reused by a future allocation. The
pointer passed to this function is no longer safe to dereference once this
function returns, and should be discarded.

## Version

This function is available since SDL 2.0.10.

## See Also

- [SDL_SIMDAlloc](SDL_SIMDAlloc)
- [SDL_SIMDRealloc](SDL_SIMDRealloc)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryCPUInfo](CategoryCPUInfo)

