# SDL_LogVerbose

Log a message with [SDL_LOG_PRIORITY_VERBOSE](SDL_LOG_PRIORITY_VERBOSE).

## Header File

Defined in [<SDL3/SDL_log.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_log.h)

## Syntax

```c
void SDL_LogVerbose(int category, const char *fmt, ...);
```

## Function Parameters

|              |              |                                                                        |
| ------------ | ------------ | ---------------------------------------------------------------------- |
| int          | **category** | the category of the message.                                           |
| const char * | **fmt**      | a printf() style message format string.                                |
| ...          | **...**      | additional parameters matching % tokens in the **fmt** string, if any. |

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
- [SDL_LogMessage](SDL_LogMessage)
- [SDL_LogMessageV](SDL_LogMessageV)
- [SDL_LogWarn](SDL_LogWarn)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLog](CategoryLog)

