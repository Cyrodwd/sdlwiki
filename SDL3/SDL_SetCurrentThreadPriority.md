###### (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)
# SDL_SetCurrentThreadPriority

Set the priority for the current thread.

## Header File

Defined in [<SDL3/SDL_thread.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_thread.h)

## Syntax

```c
bool SDL_SetCurrentThreadPriority(SDL_ThreadPriority priority);
```

## Function Parameters

|                                          |              |                                                      |
| ---------------------------------------- | ------------ | ---------------------------------------------------- |
| [SDL_ThreadPriority](SDL_ThreadPriority) | **priority** | the [SDL_ThreadPriority](SDL_ThreadPriority) to set. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Note that some platforms will not let you alter the priority (or at least,
promote the thread to a higher priority) at all, and some require you to be
an administrator account. Be prepared for this to fail.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryThread](CategoryThread)

