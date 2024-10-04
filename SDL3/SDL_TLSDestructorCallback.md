###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_TLSDestructorCallback

The callback used to cleanup data passed to [SDL_SetTLS](SDL_SetTLS).

## Header File

Defined in [<SDL3/SDL_thread.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_thread.h)

## Syntax

```c
typedef void (SDLCALL *SDL_TLSDestructorCallback)(void *value);
```

## Function Parameters

|           |                                                          |
| --------- | -------------------------------------------------------- |
| **value** | a pointer previously handed to [SDL_SetTLS](SDL_SetTLS). |

## Remarks

This is called when a thread exits, to allow an app to free any resources.

## Version

This datatype is available since SDL 3.0.0.

## See Also

- [SDL_SetTLS](SDL_SetTLS)

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryThread](CategoryThread)

