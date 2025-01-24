# SDL_LogOutputFunction

The prototype for the log output callback function.

## Header File

Defined in [<SDL3/SDL_log.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_log.h)

## Syntax

```c
typedef void (SDLCALL *SDL_LogOutputFunction)(void *userdata, int category, SDL_LogPriority priority, const char *message);
```

## Function Parameters

|              |                                                                                          |
| ------------ | ---------------------------------------------------------------------------------------- |
| **userdata** | what was passed as `userdata` to [SDL_SetLogOutputFunction](SDL_SetLogOutputFunction)(). |
| **category** | the category of the message.                                                             |
| **priority** | the priority of the message.                                                             |
| **message**  | the message being output.                                                                |

## Remarks

This function is called by SDL when there is new text to be logged. A mutex
is held so that this function is never called by more than one thread at
once.

## Version

This datatype is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryLog](CategoryLog)

