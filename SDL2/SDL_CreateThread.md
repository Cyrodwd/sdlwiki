###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_CreateThread

Create a new thread with a default stack size.

## Header File

Defined in [SDL_thread.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_thread.h)

## Syntax

```c
extern DECLSPEC SDL_Thread *SDLCALL
SDL_CreateThread(SDL_ThreadFunction fn, const char *name, void *data);
```

## Function Parameters

|                                          |          |                                                                                  |
| ---------------------------------------- | -------- | -------------------------------------------------------------------------------- |
| [SDL_ThreadFunction](SDL_ThreadFunction) | **fn**   | the [SDL_ThreadFunction](SDL_ThreadFunction) function to call in the new thread. |
| const char *                             | **name** | the name of the thread.                                                          |
| void *                                   | **data** | a pointer that is passed to `fn`.                                                |

## Return Value

([SDL_Thread](SDL_Thread) *) Returns an opaque pointer to the new thread
object on success, NULL if the new thread could not be created; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This is equivalent to calling:

```c
SDL_CreateThreadWithStackSize(fn, name, 0, data);
```

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateThreadWithStackSize](SDL_CreateThreadWithStackSize)
- [SDL_WaitThread](SDL_WaitThread)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryThread](CategoryThread)

