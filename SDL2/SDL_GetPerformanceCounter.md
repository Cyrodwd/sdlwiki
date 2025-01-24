# SDL_GetPerformanceCounter

Get the current value of the high resolution counter.

## Header File

Defined in [SDL_timer.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_timer.h)

## Syntax

```c
Uint64 SDL_GetPerformanceCounter(void);
```

## Return Value

([Uint64](Uint64)) Returns the current counter value.

## Remarks

This function is typically used for profiling.

The counter values are only meaningful relative to each other. Differences
between values can be converted to times by using
[SDL_GetPerformanceFrequency](SDL_GetPerformanceFrequency)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetPerformanceFrequency](SDL_GetPerformanceFrequency)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryTimer](CategoryTimer)

