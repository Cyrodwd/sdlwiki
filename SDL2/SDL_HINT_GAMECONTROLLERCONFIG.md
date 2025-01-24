# SDL_HINT_GAMECONTROLLERCONFIG

A variable that lets you manually hint extra gamecontroller db entries.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_GAMECONTROLLERCONFIG "SDL_GAMECONTROLLERCONFIG"
```

## Remarks

The variable should be newline delimited rows of gamecontroller config
data, see [SDL_gamecontroller](SDL_gamecontroller).h

This hint must be set before calling
[SDL_Init](SDL_Init)([SDL_INIT_GAMECONTROLLER](SDL_INIT_GAMECONTROLLER))
You can update mappings after the system is initialized with
[SDL_GameControllerMappingForGUID](SDL_GameControllerMappingForGUID)() and
[SDL_GameControllerAddMapping](SDL_GameControllerAddMapping)()





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

