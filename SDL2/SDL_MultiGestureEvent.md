# SDL_MultiGestureEvent

Multiple Finger Gesture Event (event.mgesture.*)

## Header File

Defined in [SDL_events.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_events.h)

## Syntax

```c
typedef struct SDL_MultiGestureEvent
{
    Uint32 type;        /**< SDL_MULTIGESTURE */
    Uint32 timestamp;   /**< In milliseconds, populated using SDL_GetTicks() */
    SDL_TouchID touchId; /**< The touch device id */
    float dTheta;
    float dDist;
    float x;
    float y;
    Uint16 numFingers;
    Uint16 padding;
} SDL_MultiGestureEvent;
```

----
[CategoryAPI](CategoryAPI), [CategoryAPIStruct](CategoryAPIStruct), [CategoryEvents](CategoryEvents)

