# SDL_LogGetPriority

Get the priority of a particular log category.

## Header File

Defined in [SDL_log.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_log.h)

## Syntax

```c
SDL_LogPriority SDL_LogGetPriority(int category);
```

## Function Parameters

|     |              |                        |
| --- | ------------ | ---------------------- |
| int | **category** | the category to query. |

## Return Value

([SDL_LogPriority](SDL_LogPriority)) Returns the
[SDL_LogPriority](SDL_LogPriority) for the requested category.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_LogSetPriority](SDL_LogSetPriority)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLog](CategoryLog)

