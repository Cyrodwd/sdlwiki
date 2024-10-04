###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_JoystickGetHat

Get the current state of a POV hat on a joystick.

## Header File

Defined in [SDL_joystick.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_joystick.h)

## Syntax

```c
Uint8 SDL_JoystickGetHat(SDL_Joystick *joystick,
                         int hat);
```

## Function Parameters

|                                |              |                                                                            |
| ------------------------------ | ------------ | -------------------------------------------------------------------------- |
| [SDL_Joystick](SDL_Joystick) * | **joystick** | an [SDL_Joystick](SDL_Joystick) structure containing joystick information. |
| int                            | **hat**      | the hat index to get the state from; indices start at index 0.             |

## Return Value

(Uint8) Returns the current hat position.

## Remarks

The returned value will be one of the following positions:

- [`SDL_HAT_CENTERED`](SDL_HAT_CENTERED)
- [`SDL_HAT_UP`](SDL_HAT_UP)
- [`SDL_HAT_RIGHT`](SDL_HAT_RIGHT)
- [`SDL_HAT_DOWN`](SDL_HAT_DOWN)
- [`SDL_HAT_LEFT`](SDL_HAT_LEFT)
- [`SDL_HAT_RIGHTUP`](SDL_HAT_RIGHTUP)
- [`SDL_HAT_RIGHTDOWN`](SDL_HAT_RIGHTDOWN)
- [`SDL_HAT_LEFTUP`](SDL_HAT_LEFTUP)
- [`SDL_HAT_LEFTDOWN`](SDL_HAT_LEFTDOWN)

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_JoystickNumHats](SDL_JoystickNumHats)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryJoystick](CategoryJoystick)

