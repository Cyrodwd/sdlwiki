# SDL_LogMessage

Log a message with the specified category and priority.

## Header File

Defined in [<SDL3/SDL_log.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_log.h)

## Syntax

```c
void SDL_LogMessage(int category,
                SDL_LogPriority priority,
                const char *fmt, ...);
```

## Function Parameters

|                                    |              |                                                                        |
| ---------------------------------- | ------------ | ---------------------------------------------------------------------- |
| int                                | **category** | the category of the message.                                           |
| [SDL_LogPriority](SDL_LogPriority) | **priority** | the priority of the message.                                           |
| const char *                       | **fmt**      | a printf() style message format string.                                |
| ...                                | **...**      | additional parameters matching % tokens in the **fmt** string, if any. |

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_Log](SDL_Log)
- [SDL_LogCritical](SDL_LogCritical)
- [SDL_LogDebug](SDL_LogDebug)
- [SDL_LogError](SDL_LogError)
- [SDL_LogInfo](SDL_LogInfo)
- [SDL_LogMessageV](SDL_LogMessageV)
- [SDL_LogTrace](SDL_LogTrace)
- [SDL_LogVerbose](SDL_LogVerbose)
- [SDL_LogWarn](SDL_LogWarn)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLog](CategoryLog)

