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

This datatype is available since SDL 3.2.0.

## See Also

- [SDL_SetTLS](SDL_SetTLS)

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryThread](CategoryThread)

