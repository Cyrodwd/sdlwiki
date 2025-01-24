# SDL_GetThreadName

Get the thread name as it was specified in [SDL_CreateThread](SDL_CreateThread)().

## Header File

Defined in [<SDL3/SDL_thread.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_thread.h)

## Syntax

```c
const char * SDL_GetThreadName(SDL_Thread *thread);
```

## Function Parameters

|                            |            |                      |
| -------------------------- | ---------- | -------------------- |
| [SDL_Thread](SDL_Thread) * | **thread** | the thread to query. |

## Return Value

(const char *) Returns a pointer to a UTF-8 string that names the specified
thread, or NULL if it doesn't have a name.

## Version

This function is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryThread](CategoryThread)

