# SDL_LogError

Log a message with [SDL_LOG_PRIORITY_ERROR](SDL_LOG_PRIORITY_ERROR).

## Header File

Defined in [SDL_log.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_log.h)

## Syntax

```c
void SDL_LogError(int category, const char *fmt, ...);
```

## Function Parameters

|              |              |                                                                        |
| ------------ | ------------ | ---------------------------------------------------------------------- |
| int          | **category** | the category of the message.                                           |
| const char * | **fmt**      | a printf() style message format string.                                |
| ...          | **...**      | additional parameters matching % tokens in the **fmt** string, if any. |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_Log](SDL_Log)
- [SDL_LogCritical](SDL_LogCritical)
- [SDL_LogDebug](SDL_LogDebug)
- [SDL_LogInfo](SDL_LogInfo)
- [SDL_LogMessage](SDL_LogMessage)
- [SDL_LogMessageV](SDL_LogMessageV)
- [SDL_LogVerbose](SDL_LogVerbose)
- [SDL_LogWarn](SDL_LogWarn)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLog](CategoryLog)

