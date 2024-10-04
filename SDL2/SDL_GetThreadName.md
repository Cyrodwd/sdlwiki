###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetThreadName

Get the thread name as it was specified in [SDL_CreateThread](SDL_CreateThread)().

## Header File

Defined in [SDL_thread.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_thread.h)

## Syntax

```c
const char* SDL_GetThreadName(SDL_Thread *thread);
```

## Function Parameters

|                            |            |                      |
| -------------------------- | ---------- | -------------------- |
| [SDL_Thread](SDL_Thread) * | **thread** | the thread to query. |

## Return Value

(const char *) Returns a pointer to a UTF-8 string that names the specified
thread, or NULL if it doesn't have a name.

## Remarks

This is internal memory, not to be freed by the caller, and remains valid
until the specified thread is cleaned up by
[SDL_WaitThread](SDL_WaitThread)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateThread](SDL_CreateThread)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryThread](CategoryThread)

