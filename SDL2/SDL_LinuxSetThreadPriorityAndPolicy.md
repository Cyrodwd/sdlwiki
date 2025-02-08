# SDL_LinuxSetThreadPriorityAndPolicy

Sets the priority (not nice level) and scheduling policy for a thread.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
int SDL_LinuxSetThreadPriorityAndPolicy(Sint64 threadID, int sdlPriority, int schedPolicy);
```

## Function Parameters

|                  |                 |                                                                        |
| ---------------- | --------------- | ---------------------------------------------------------------------- |
| [Sint64](Sint64) | **threadID**    | The Unix thread ID to change priority of.                              |
| int              | **sdlPriority** | The new [SDL_ThreadPriority](SDL_ThreadPriority) value.                |
| int              | **schedPolicy** | The new scheduling policy (SCHED_FIFO, SCHED_RR, SCHED_OTHER, etc...). |

## Return Value

(int) Returns 0 on success, or -1 on error.

## Remarks

This uses setpriority() if possible, and RealtimeKit if available.

## Version

This function is available since SDL 2.0.18.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

