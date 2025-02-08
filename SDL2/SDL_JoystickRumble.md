# SDL_JoystickRumble

Start a rumble effect.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
int SDL_JoystickRumble(SDL_Joystick *joystick, Uint16 low_frequency_rumble, Uint16 high_frequency_rumble, Uint32 duration_ms);
```

## Function Parameters

|                                |                           |                                                                             |
| ------------------------------ | ------------------------- | --------------------------------------------------------------------------- |
| [SDL_Joystick](SDL_Joystick) * | **joystick**              | The joystick to vibrate.                                                    |
| [Uint16](Uint16)               | **low_frequency_rumble**  | The intensity of the low frequency (left) rumble motor, from 0 to 0xFFFF.   |
| [Uint16](Uint16)               | **high_frequency_rumble** | The intensity of the high frequency (right) rumble motor, from 0 to 0xFFFF. |
| [Uint32](Uint32)               | **duration_ms**           | The duration of the rumble effect, in milliseconds.                         |

## Return Value

(int) Returns 0, or -1 if rumble isn't supported on this joystick.

## Remarks

Each call to this function cancels any previous rumble effect, and calling
it with 0 intensity stops any rumbling.

## Version

This function is available since SDL 2.0.9.

## See Also

- [SDL_JoystickHasRumble](SDL_JoystickHasRumble)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

