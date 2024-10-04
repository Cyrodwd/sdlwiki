###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HapticName

Get the implementation dependent name of a haptic device.

## Header File

Defined in [SDL_haptic.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_haptic.h)

## Syntax

```c
const char* SDL_HapticName(int device_index);
```

## Function Parameters

|     |                  |                               |
| --- | ---------------- | ----------------------------- |
| int | **device_index** | index of the device to query. |

## Return Value

(const char *) Returns the name of the device or NULL on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This can be called before any joysticks are opened. If no name can be
found, this function returns NULL.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_NumHaptics](SDL_NumHaptics)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHaptic](CategoryHaptic)

