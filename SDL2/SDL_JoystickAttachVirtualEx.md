###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_JoystickAttachVirtualEx

Attach a new virtual joystick with extended properties.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
int SDL_JoystickAttachVirtualEx(const SDL_VirtualJoystickDesc *desc);
```

## Return Value

(int) Returns the joystick's device index, or -1 if an error occurred.

## Version

This function is available since SDL 2.24.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

