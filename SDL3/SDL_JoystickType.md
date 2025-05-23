# SDL_JoystickType

An enum of some common joystick types.

## Header File

Defined in [<SDL3/SDL_joystick.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_joystick.h)

## Syntax

```c
typedef enum SDL_JoystickType
{
    SDL_JOYSTICK_TYPE_UNKNOWN,
    SDL_JOYSTICK_TYPE_GAMEPAD,
    SDL_JOYSTICK_TYPE_WHEEL,
    SDL_JOYSTICK_TYPE_ARCADE_STICK,
    SDL_JOYSTICK_TYPE_FLIGHT_STICK,
    SDL_JOYSTICK_TYPE_DANCE_PAD,
    SDL_JOYSTICK_TYPE_GUITAR,
    SDL_JOYSTICK_TYPE_DRUM_KIT,
    SDL_JOYSTICK_TYPE_ARCADE_PAD,
    SDL_JOYSTICK_TYPE_THROTTLE,
    SDL_JOYSTICK_TYPE_COUNT
} SDL_JoystickType;
```

## Remarks

In some cases, SDL can identify a low-level joystick as being a certain
type of device, and will report it through
[SDL_GetJoystickType](SDL_GetJoystickType) (or
[SDL_GetJoystickTypeForID](SDL_GetJoystickTypeForID)).

This is by no means a complete list of everything that can be plugged into
a computer.

You may refer to
[XInput Controller Types](https://learn.microsoft.com/en-us/windows/win32/xinput/xinput-and-controller-subtypes)
table for a general understanding of each joystick type.

## Version

This enum is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIEnum](CategoryAPIEnum), [CategoryJoystick](CategoryJoystick)

