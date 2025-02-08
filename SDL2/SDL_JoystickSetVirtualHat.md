# SDL_JoystickSetVirtualHat

Set values on an opened, virtual-joystick's hat.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
int SDL_JoystickSetVirtualHat(SDL_Joystick *joystick, int hat, Uint8 value);
```

## Function Parameters

|                                |              |                                                  |
| ------------------------------ | ------------ | ------------------------------------------------ |
| [SDL_Joystick](SDL_Joystick) * | **joystick** | the virtual joystick on which to set state.      |
| int                            | **hat**      | the specific hat on the virtual joystick to set. |
| Uint8                          | **value**    | the new value for the specified hat.             |

## Return Value

(int) Returns 0 on success, -1 on error.

## Remarks

Please note that values set here will not be applied until the next call to
[SDL_JoystickUpdate](SDL_JoystickUpdate), which can either be called
directly, or can be called indirectly through various other SDL APIs,
including, but not limited to the following:
[SDL_PollEvent](SDL_PollEvent), [SDL_PumpEvents](SDL_PumpEvents),
[SDL_WaitEventTimeout](SDL_WaitEventTimeout),
[SDL_WaitEvent](SDL_WaitEvent).

## Version

This function is available since SDL 2.0.14.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

