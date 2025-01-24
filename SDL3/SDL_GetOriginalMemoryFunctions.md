# SDL_GetOriginalMemoryFunctions

Get the original set of SDL memory functions.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
void SDL_GetOriginalMemoryFunctions(SDL_malloc_func *malloc_func,
                                SDL_calloc_func *calloc_func,
                                SDL_realloc_func *realloc_func,
                                SDL_free_func *free_func);
```

## Function Parameters

|                                        |                  |                               |
| -------------------------------------- | ---------------- | ----------------------------- |
| [SDL_malloc_func](SDL_malloc_func) *   | **malloc_func**  | filled with malloc function.  |
| [SDL_calloc_func](SDL_calloc_func) *   | **calloc_func**  | filled with calloc function.  |
| [SDL_realloc_func](SDL_realloc_func) * | **realloc_func** | filled with realloc function. |
| [SDL_free_func](SDL_free_func) *       | **free_func**    | filled with free function.    |

## Remarks

This is what [SDL_malloc](SDL_malloc) and friends will use by default, if
there has been no call to [SDL_SetMemoryFunctions](SDL_SetMemoryFunctions).
This is not necessarily using the C runtime's `malloc` functions behind the
scenes! Different platforms and build configurations might do any number of
unexpected things.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

