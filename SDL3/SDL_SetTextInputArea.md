###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_SetTextInputArea

Set the area used to type Unicode text input.

## Header File

Defined in [<SDL3/SDL_keyboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_keyboard.h)

## Syntax

```c
bool SDL_SetTextInputArea(SDL_Window *window, const SDL_Rect *rect, int cursor);
```

## Function Parameters

|                              |            |                                                                                                        |
| ---------------------------- | ---------- | ------------------------------------------------------------------------------------------------------ |
| [SDL_Window](SDL_Window) *   | **window** | the window for which to set the text input area.                                                       |
| const [SDL_Rect](SDL_Rect) * | **rect**   | the [SDL_Rect](SDL_Rect) representing the text input area, in window coordinates, or NULL to clear it. |
| int                          | **cursor** | the offset of the current cursor location relative to `rect->x`, in window coordinates.                |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Native input methods may place a window with word suggestions near the
cursor, without covering the text being entered.

## Thread Safety

This function should only be called on the main thread.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_GetTextInputArea](SDL_GetTextInputArea)
- [SDL_StartTextInput](SDL_StartTextInput)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

