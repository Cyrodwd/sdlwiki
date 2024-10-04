###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_iOSAnimationCallback

The prototype for an Apple iOS animation callback.

## Header File

Defined in [<SDL3/SDL_system.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_system.h)

## Syntax

```c
typedef void (SDLCALL *SDL_iOSAnimationCallback)(void *userdata);
```

## Function Parameters

|              |                                                                                                                      |
| ------------ | -------------------------------------------------------------------------------------------------------------------- |
| **userdata** | what was passed as `callbackParam` to [SDL_SetiOSAnimationCallback](SDL_SetiOSAnimationCallback) as `callbackParam`. |

## Remarks

This datatype is only useful on Apple iOS.

After passing a function pointer of this type to
[SDL_SetiOSAnimationCallback](SDL_SetiOSAnimationCallback), the system will
call that function pointer at a regular interval.

## Version

This datatype is available since SDL 3.0.0.

## See Also

- [SDL_SetiOSAnimationCallback](SDL_SetiOSAnimationCallback)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategorySystem](CategorySystem)

