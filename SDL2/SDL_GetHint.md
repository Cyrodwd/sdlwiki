# SDL_GetHint

Get the value of a hint.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
const char * SDL_GetHint(const char *name);
```

## Function Parameters

|              |          |                    |
| ------------ | -------- | ------------------ |
| const char * | **name** | the hint to query. |

## Return Value

(const char *) Returns the string value of a hint or NULL if the hint isn't
set.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetHint](SDL_SetHint)
- [SDL_SetHintWithPriority](SDL_SetHintWithPriority)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHints](CategoryHints)

