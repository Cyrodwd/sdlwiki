# SDL_TimerCallback

Function prototype for the millisecond timer callback function.

## Header File

Defined in [<SDL3/SDL_timer.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_timer.h)

## Syntax

```c
typedef Uint32 (SDLCALL *SDL_TimerCallback)(void *userdata, SDL_TimerID timerID, Uint32 interval);
```

## Function Parameters

|              |                                                                                                 |
| ------------ | ----------------------------------------------------------------------------------------------- |
| **userdata** | an arbitrary pointer provided by the app through [SDL_AddTimer](SDL_AddTimer), for its own use. |
| **timerID**  | the current timer being processed.                                                              |
| **interval** | the current callback time interval.                                                             |

## Return Value

Returns the new callback time interval, or 0 to disable further runs of the
callback.

## Remarks

The callback function is passed the current timer interval and returns the
next timer interval, in milliseconds. If the returned value is the same as
the one passed in, the periodic alarm continues, otherwise a new alarm is
scheduled. If the callback returns 0, the periodic alarm is canceled and
will be removed.

## Thread Safety

SDL may call this callback at any time from a background thread; the
application is responsible for locking resources the callback touches that
need to be protected.

## Version

This datatype is available since SDL 3.2.0.

## See Also

- [SDL_AddTimer](SDL_AddTimer)






----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryTimer](CategoryTimer)

