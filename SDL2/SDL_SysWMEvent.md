###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_SysWMEvent

A video driver dependent system event (event.syswm.*)

## Header File

Defined in [SDL_events.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_events.h)

## Syntax

```c
typedef struct SDL_SysWMEvent
{
    Uint32 type;        /**< SDL_SYSWMEVENT */
    Uint32 timestamp;   /**< In milliseconds, populated using SDL_GetTicks() */
    SDL_SysWMmsg *msg;  /**< driver dependent data, defined in SDL_syswm.h */
} SDL_SysWMEvent;
```

## Remarks

This event is disabled by default, you can enable it with
[SDL_EventState](SDL_EventState)()

If you want to use this event, you should include [SDL_syswm](SDL_syswm).h.

----
[CategoryAPI](CategoryAPI), [CategoryAPIStruct](CategoryAPIStruct), [CategoryEvents](CategoryEvents)

