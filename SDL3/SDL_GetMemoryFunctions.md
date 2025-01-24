# SDL_GetMemoryFunctions

Get the current set of SDL memory functions.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
void SDL_GetMemoryFunctions(SDL_malloc_func *malloc_func,
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

## Thread Safety

This does not hold a lock, so do not call this in the unlikely event of a
background thread calling [SDL_SetMemoryFunctions](SDL_SetMemoryFunctions)
simultaneously.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_SetMemoryFunctions](SDL_SetMemoryFunctions)
- [SDL_GetOriginalMemoryFunctions](SDL_GetOriginalMemoryFunctions)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

