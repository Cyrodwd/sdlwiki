###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SetHintWithPriority

Set a hint with a specific priority.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
SDL_bool SDL_SetHintWithPriority(const char *name,
                                 const char *value,
                                 SDL_HintPriority priority);
```

## Function Parameters

|                                      |              |                                                              |
| ------------------------------------ | ------------ | ------------------------------------------------------------ |
| const char *                         | **name**     | the hint to set.                                             |
| const char *                         | **value**    | the value of the hint variable.                              |
| [SDL_HintPriority](SDL_HintPriority) | **priority** | the [SDL_HintPriority](SDL_HintPriority) level for the hint. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if the hint was set,
[SDL_FALSE](SDL_FALSE) otherwise.

## Remarks

The priority controls the behavior when setting a hint that already has a
value. Hints will replace existing hints of their priority and lower.
Environment variables are considered to have override priority.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetHint](SDL_GetHint)
- [SDL_SetHint](SDL_SetHint)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHints](CategoryHints)

