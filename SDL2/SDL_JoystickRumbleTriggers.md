###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_JoystickRumbleTriggers

Start a rumble effect in the joystick's triggers

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
int SDL_JoystickRumbleTriggers(SDL_Joystick *joystick, Uint16 left_rumble, Uint16 right_rumble, Uint32 duration_ms);
```

## Function Parameters

|                                |                  |                                                                    |
| ------------------------------ | ---------------- | ------------------------------------------------------------------ |
| [SDL_Joystick](SDL_Joystick) * | **joystick**     | The joystick to vibrate.                                           |
| [Uint16](Uint16)               | **left_rumble**  | The intensity of the left trigger rumble motor, from 0 to 0xFFFF.  |
| [Uint16](Uint16)               | **right_rumble** | The intensity of the right trigger rumble motor, from 0 to 0xFFFF. |
| [Uint32](Uint32)               | **duration_ms**  | The duration of the rumble effect, in milliseconds.                |

## Return Value

(int) Returns 0, or -1 if trigger rumble isn't supported on this joystick.

## Remarks

Each call to this function cancels any previous trigger rumble effect, and
calling it with 0 intensity stops any rumbling.

Note that this is rumbling of the _triggers_ and not the game controller as
a whole. This is currently only supported on Xbox One controllers. If you
want the (more common) whole-controller rumble, use
[SDL_JoystickRumble](SDL_JoystickRumble)() instead.

## Version

This function is available since SDL 2.0.14.

## See Also

- [SDL_JoystickHasRumbleTriggers](SDL_JoystickHasRumbleTriggers)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

