# SDL_ResetLogPriorities

Reset all priorities to default.

## Header File

Defined in [<SDL3/SDL_log.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_log.h)

## Syntax

```c
void SDL_ResetLogPriorities(void);
```

## Remarks

This is called by [SDL_Quit](SDL_Quit)().

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_SetLogPriorities](SDL_SetLogPriorities)
- [SDL_SetLogPriority](SDL_SetLogPriority)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLog](CategoryLog)

