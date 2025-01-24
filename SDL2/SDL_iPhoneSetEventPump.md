# SDL_iPhoneSetEventPump

Use this function to enable or disable the SDL event pump on Apple iOS.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
void SDL_iPhoneSetEventPump(SDL_bool enabled);


#define SDL_iOSSetEventPump(enabled) SDL_iPhoneSetEventPump(enabled)
```

## Function Parameters

|                      |             |                                                                                      |
| -------------------- | ----------- | ------------------------------------------------------------------------------------ |
| [SDL_bool](SDL_bool) | **enabled** | [SDL_TRUE](SDL_TRUE) to enable the event pump, [SDL_FALSE](SDL_FALSE) to disable it. |

## Remarks

This function is only available on Apple iOS.

This functions is also accessible using the macro
[SDL_iOSSetEventPump](SDL_iOSSetEventPump)() since SDL 2.0.4.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_iPhoneSetAnimationCallback](SDL_iPhoneSetAnimationCallback)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

