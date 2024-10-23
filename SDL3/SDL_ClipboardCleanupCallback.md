###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_ClipboardCleanupCallback

Callback function that will be called when the clipboard is cleared, or new data is set.

## Header File

Defined in [<SDL3/SDL_clipboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_clipboard.h)

## Syntax

```c
typedef void (SDLCALL *SDL_ClipboardCleanupCallback)(void *userdata);
```

## Function Parameters

|              |                                  |
| ------------ | -------------------------------- |
| **userdata** | a pointer to provided user data. |

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_SetClipboardData](SDL_SetClipboardData)

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryClipboard](CategoryClipboard)

