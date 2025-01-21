###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_HINT_GAMECONTROLLERCONFIG

A variable that lets you manually hint extra gamecontroller db entries.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_GAMECONTROLLERCONFIG "SDL_GAMECONTROLLERCONFIG"
```

## Remarks

The variable should be newline delimited rows of gamecontroller config
data, see [SDL_gamepad](SDL_gamepad).h

You can update mappings after SDL is initialized with
[SDL_GetGamepadMappingForGUID](SDL_GetGamepadMappingForGUID)() and
[SDL_AddGamepadMapping](SDL_AddGamepadMapping)()

This hint should be set before SDL is initialized.

## Version

This hint is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

