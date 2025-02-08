# SDL_GetNumTouchFingers

Get the number of active fingers for a given touch device.

## Header File

Defined in [SDL_touch.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_touch.h)

## Syntax

```c
int SDL_GetNumTouchFingers(SDL_TouchID touchID);
```

## Function Parameters

|                            |             |                           |
| -------------------------- | ----------- | ------------------------- |
| [SDL_TouchID](SDL_TouchID) | **touchID** | the ID of a touch device. |

## Return Value

(int) Returns the number of active fingers for a given touch device on
success or 0 on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetTouchFinger](SDL_GetTouchFinger)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryTouch](CategoryTouch)

