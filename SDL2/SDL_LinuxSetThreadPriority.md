# SDL_LinuxSetThreadPriority

Sets the UNIX nice value for a thread.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
int SDL_LinuxSetThreadPriority(Sint64 threadID, int priority);
```

## Function Parameters

|                  |              |                                           |
| ---------------- | ------------ | ----------------------------------------- |
| [Sint64](Sint64) | **threadID** | the Unix thread ID to change priority of. |
| int              | **priority** | The new, Unix-specific, priority value.   |

## Return Value

(int) Returns 0 on success, or -1 on error.

## Remarks

This uses setpriority() if possible, and RealtimeKit if available.

## Version

This function is available since SDL 2.0.9.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

