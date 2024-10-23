###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetPrimarySelectionText

Get UTF-8 text from the primary selection.

## Header File

Defined in [<SDL3/SDL_clipboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_clipboard.h)

## Syntax

```c
char * SDL_GetPrimarySelectionText(void);
```

## Return Value

(char *) Returns the primary selection text on success or an empty string
on failure; call [SDL_GetError](SDL_GetError)() for more information. This
should be freed with [SDL_free](SDL_free)() when it is no longer needed.

## Remarks

This functions returns an empty string if there was not enough memory left
for a copy of the primary selection's content.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_HasPrimarySelectionText](SDL_HasPrimarySelectionText)
- [SDL_SetPrimarySelectionText](SDL_SetPrimarySelectionText)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryClipboard](CategoryClipboard)

