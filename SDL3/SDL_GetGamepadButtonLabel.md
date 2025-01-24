# SDL_GetGamepadButtonLabel

Get the label of a button on a gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
SDL_GamepadButtonLabel SDL_GetGamepadButtonLabel(SDL_Gamepad *gamepad, SDL_GamepadButton button);
```

## Function Parameters

|                                        |             |                                                                            |
| -------------------------------------- | ----------- | -------------------------------------------------------------------------- |
| [SDL_Gamepad](SDL_Gamepad) *           | **gamepad** | a gamepad.                                                                 |
| [SDL_GamepadButton](SDL_GamepadButton) | **button**  | a button index (one of the [SDL_GamepadButton](SDL_GamepadButton) values). |

## Return Value

([SDL_GamepadButtonLabel](SDL_GamepadButtonLabel)) Returns the
[SDL_GamepadButtonLabel](SDL_GamepadButtonLabel) enum corresponding to the
button label.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetGamepadButtonLabelForType](SDL_GetGamepadButtonLabelForType)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

