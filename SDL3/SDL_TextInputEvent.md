# SDL_TextInputEvent

Keyboard text input event structure (event.text.*)

## Header File

Defined in [<SDL3/SDL_events.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_events.h)

## Syntax

```c
typedef struct SDL_TextInputEvent
{
    SDL_EventType type; /**< SDL_EVENT_TEXT_INPUT */
    Uint32 reserved;
    Uint64 timestamp;   /**< In nanoseconds, populated using SDL_GetTicksNS() */
    SDL_WindowID windowID; /**< The window with keyboard focus, if any */
    const char *text;   /**< The input text, UTF-8 encoded */
} SDL_TextInputEvent;
```

## Remarks

This event will never be delivered unless text input is enabled by calling
[SDL_StartTextInput](SDL_StartTextInput)(). Text input is disabled by
default!

## Version

This struct is available since SDL 3.2.0.

## See Also

- [SDL_StartTextInput](SDL_StartTextInput)
- [SDL_StopTextInput](SDL_StopTextInput)

----
[CategoryAPI](CategoryAPI), [CategoryAPIStruct](CategoryAPIStruct), [CategoryEvents](CategoryEvents)

