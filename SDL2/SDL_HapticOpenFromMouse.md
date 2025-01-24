# SDL_HapticOpenFromMouse

Try to open a haptic device from the current mouse.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
SDL_Haptic* SDL_HapticOpenFromMouse(void);
```

## Return Value

([SDL_Haptic](SDL_Haptic) *) Returns the haptic device identifier or NULL
on failure; call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_HapticOpen](SDL_HapticOpen)
- [SDL_MouseIsHaptic](SDL_MouseIsHaptic)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

