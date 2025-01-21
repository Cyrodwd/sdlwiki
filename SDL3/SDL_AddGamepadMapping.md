###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_AddGamepadMapping

Add support for gamepads that SDL is unaware of or change the binding of an existing gamepad.

## Header File

Defined in [<SDL3/SDL_gamepad.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_gamepad.h)

## Syntax

```c
int SDL_AddGamepadMapping(const char *mapping);
```

## Function Parameters

|              |             |                     |
| ------------ | ----------- | ------------------- |
| const char * | **mapping** | the mapping string. |

## Return Value

(int) Returns 1 if a new mapping is added, 0 if an existing mapping is
updated, -1 on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

The mapping string has the format "GUID,name,mapping", where GUID is the
string value from [SDL_GUIDToString](SDL_GUIDToString)(), name is the human
readable string for the device and mappings are gamepad mappings to
joystick ones. Under Windows there is a reserved GUID of "xinput" that
covers all XInput devices. The mapping format for joystick is:

- `bX`: a joystick button, index X
- `hX.Y`: hat X with value Y
- `aX`: axis X of the joystick

Buttons can be used as a gamepad axes and vice versa.

If a device with this GUID is already plugged in, SDL will generate an
[SDL_EVENT_GAMEPAD_ADDED](SDL_EVENT_GAMEPAD_ADDED) event.

This string shows an example of a valid mapping for a gamepad:

```c
"341a3608000000000000504944564944,Afterglow PS3 Controller,a:b1,b:b2,y:b3,x:b0,start:b9,guide:b12,back:b8,dpup:h0.1,dpleft:h0.8,dpdown:h0.4,dpright:h0.2,leftshoulder:b4,rightshoulder:b5,leftstick:b10,rightstick:b11,leftx:a0,lefty:a1,rightx:a2,righty:a3,lefttrigger:b6,righttrigger:b7"
```

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_AddGamepadMappingsFromFile](SDL_AddGamepadMappingsFromFile)
- [SDL_AddGamepadMappingsFromIO](SDL_AddGamepadMappingsFromIO)
- [SDL_GetGamepadMapping](SDL_GetGamepadMapping)
- [SDL_GetGamepadMappingForGUID](SDL_GetGamepadMappingForGUID)
- [SDL_HINT_GAMECONTROLLERCONFIG](SDL_HINT_GAMECONTROLLERCONFIG)
- [SDL_HINT_GAMECONTROLLERCONFIG_FILE](SDL_HINT_GAMECONTROLLERCONFIG_FILE)
- [SDL_EVENT_GAMEPAD_ADDED](SDL_EVENT_GAMEPAD_ADDED)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGamepad](CategoryGamepad)

