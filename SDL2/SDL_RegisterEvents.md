# SDL_RegisterEvents

Allocate a set of user-defined events, and return the beginning event number for that set of events.

## Header File

Defined in [SDL_events.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_events.h)

## Syntax

```c
Uint32 SDL_RegisterEvents(int numevents);
```

## Function Parameters

|     |               |                                       |
| --- | ------------- | ------------------------------------- |
| int | **numevents** | the number of events to be allocated. |

## Return Value

([Uint32](Uint32)) Returns the beginning event number, or
([Uint32](Uint32))-1 if there are not enough user-defined events left.

## Remarks

Calling this function with `numevents` <= 0 is an error and will return
([Uint32](Uint32))-1.

Note, ([Uint32](Uint32))-1 means the maximum unsigned 32-bit integer value
(or 0xFFFFFFFF), but is clearer to write.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_PushEvent](SDL_PushEvent)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryEvents](CategoryEvents)

