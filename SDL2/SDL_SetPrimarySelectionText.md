# SDL_SetPrimarySelectionText

Put UTF-8 text into the primary selection.

## Header File

Defined in [SDL_clipboard.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_clipboard.h)

## Syntax

```c
int SDL_SetPrimarySelectionText(const char *text);
```

## Function Parameters

|              |          |                                             |
| ------------ | -------- | ------------------------------------------- |
| const char * | **text** | the text to store in the primary selection. |

## Return Value

(int) Returns 0 on success or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.26.0.

## See Also

- [SDL_GetPrimarySelectionText](SDL_GetPrimarySelectionText)
- [SDL_HasPrimarySelectionText](SDL_HasPrimarySelectionText)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryClipboard](CategoryClipboard)

