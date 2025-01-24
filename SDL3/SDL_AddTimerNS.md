# SDL_AddTimerNS

Call a callback function at a future time.

## Header File

Defined in [<SDL3/SDL_timer.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_timer.h)

## Syntax

```c
SDL_TimerID SDL_AddTimerNS(Uint64 interval, SDL_NSTimerCallback callback, void *userdata);
```

## Function Parameters

|                                            |              |                                                                                                    |
| ------------------------------------------ | ------------ | -------------------------------------------------------------------------------------------------- |
| [Uint64](Uint64)                           | **interval** | the timer delay, in nanoseconds, passed to `callback`.                                             |
| [SDL_NSTimerCallback](SDL_NSTimerCallback) | **callback** | the [SDL_TimerCallback](SDL_TimerCallback) function to call when the specified `interval` elapses. |
| void *                                     | **userdata** | a pointer that is passed to `callback`.                                                            |

## Return Value

([SDL_TimerID](SDL_TimerID)) Returns a timer ID or 0 on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

The callback function is passed the current timer interval and the user
supplied parameter from the [SDL_AddTimerNS](SDL_AddTimerNS)() call and
should return the next timer interval. If the value returned from the
callback is 0, the timer is canceled and will be removed.

The callback is run on a separate thread, and for short timeouts can
potentially be called before this function returns.

Timers take into account the amount of time it took to execute the
callback. For example, if the callback took 250 ns to execute and returned
1000 (ns), the timer would only wait another 750 ns before its next
iteration.

Timing may be inexact due to OS scheduling. Be sure to note the current
time with [SDL_GetTicksNS](SDL_GetTicksNS)() or
[SDL_GetPerformanceCounter](SDL_GetPerformanceCounter)() in case your
callback needs to adjust for variances.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_AddTimer](SDL_AddTimer)
- [SDL_RemoveTimer](SDL_RemoveTimer)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryTimer](CategoryTimer)

