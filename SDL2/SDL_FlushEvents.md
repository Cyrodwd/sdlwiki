###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_FlushEvents

Clear events of a range of types from the event queue.

## Header File

Defined in [SDL_events.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_events.h)

## Syntax

```c
void SDL_FlushEvents(Uint32 minType, Uint32 maxType);
```

## Function Parameters

|                  |             |                                                                                                      |
| ---------------- | ----------- | ---------------------------------------------------------------------------------------------------- |
| [Uint32](Uint32) | **minType** | the low end of event type to be cleared, inclusive; see [SDL_EventType](SDL_EventType) for details.  |
| [Uint32](Uint32) | **maxType** | the high end of event type to be cleared, inclusive; see [SDL_EventType](SDL_EventType) for details. |

## Remarks

This will unconditionally remove any events from the queue that are in the
range of `minType` to `maxType`, inclusive. If you need to remove a single
event type, use [SDL_FlushEvent](SDL_FlushEvent)() instead.

It's also normal to just ignore events you don't care about in your event
loop without calling this function.

This function only affects currently queued events. If you want to make
sure that all pending OS events are flushed, you can call
[SDL_PumpEvents](SDL_PumpEvents)() on the main thread immediately before
the flush call.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_FlushEvent](SDL_FlushEvent)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryEvents](CategoryEvents)

