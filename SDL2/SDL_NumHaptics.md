###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_NumHaptics

Count the number of haptic devices attached to the system.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
int SDL_NumHaptics(void);
```

## Return Value

(int) Returns the number of haptic devices detected on the system or a
negative error code on failure; call [SDL_GetError](SDL_GetError)() for
more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticName](SDL_HapticName)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

