# SDL_SetHint

Set a hint with normal priority.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
SDL_bool SDL_SetHint(const char *name,
                     const char *value);
```

## Function Parameters

|              |           |                                 |
| ------------ | --------- | ------------------------------- |
| const char * | **name**  | the hint to set.                |
| const char * | **value** | the value of the hint variable. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if the hint was set,
[SDL_FALSE](SDL_FALSE) otherwise.

## Remarks

Hints will not be set if there is an existing override hint or environment
variable that takes precedence. You can use
[SDL_SetHintWithPriority](SDL_SetHintWithPriority)() to set the hint with
override priority instead.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetHint](SDL_GetHint)
- [SDL_SetHintWithPriority](SDL_SetHintWithPriority)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHints](CategoryHints)

