# SDL_GetScancodeName

Get a human-readable name for a scancode.

## Header File

Defined in [<SDL3/SDL_keyboard.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_keyboard.h)

## Syntax

```c
const char * SDL_GetScancodeName(SDL_Scancode scancode);
```

## Function Parameters

|                              |              |                                                    |
| ---------------------------- | ------------ | -------------------------------------------------- |
| [SDL_Scancode](SDL_Scancode) | **scancode** | the desired [SDL_Scancode](SDL_Scancode) to query. |

## Return Value

(const char *) Returns a pointer to the name for the scancode. If the
scancode doesn't have a name this function returns an empty string ("").

## Remarks

**Warning**: The returned name is by design not stable across platforms,
e.g. the name for [`SDL_SCANCODE_LGUI`](SDL_SCANCODE_LGUI) is "Left GUI"
under Linux but "Left Windows" under Microsoft Windows, and some scancodes
like [`SDL_SCANCODE_NONUSBACKSLASH`](SDL_SCANCODE_NONUSBACKSLASH) don't
have any name at all. There are even scancodes that share names, e.g.
[`SDL_SCANCODE_RETURN`](SDL_SCANCODE_RETURN) and
[`SDL_SCANCODE_RETURN2`](SDL_SCANCODE_RETURN2) (both called "Return"). This
function is therefore unsuitable for creating a stable cross-platform
two-way mapping between strings and scancodes.

## Thread Safety

This function is not thread safe.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetScancodeFromKey](SDL_GetScancodeFromKey)
- [SDL_GetScancodeFromName](SDL_GetScancodeFromName)
- [SDL_SetScancodeName](SDL_SetScancodeName)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryKeyboard](CategoryKeyboard)

