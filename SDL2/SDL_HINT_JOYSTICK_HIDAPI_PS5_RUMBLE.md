###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HINT_JOYSTICK_HIDAPI_PS5_RUMBLE

A variable controlling whether extended input reports should be used for PS5 controllers when using the HIDAPI driver.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_JOYSTICK_HIDAPI_PS5_RUMBLE "SDL_JOYSTICK_HIDAPI_PS5_RUMBLE"
```

## Remarks

This variable can be set to the following values:

- "0": extended reports are not enabled (the default)
- "1": extended reports

Extended input reports allow rumble on Bluetooth PS5 controllers, but break
DirectInput handling for applications that don't use SDL.

Once extended reports are enabled, they can not be disabled without power
cycling the controller.

For compatibility with applications written for versions of SDL prior to
the introduction of PS5 controller support, this value defaults to the
value of
[SDL_HINT_JOYSTICK_HIDAPI_PS4_RUMBLE](SDL_HINT_JOYSTICK_HIDAPI_PS4_RUMBLE).

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

