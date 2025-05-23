# SDL_SetMainReady

Circumvent failure of [SDL_Init](SDL_Init)() when not using [SDL_main](SDL_main)() as an entry point.

## Header File

Defined in [SDL_main.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_main.h)

## Syntax

```c
void SDL_SetMainReady(void);
```

## Remarks

This function is defined in [SDL_main](SDL_main).h, along with the
preprocessor rule to redefine main() as [SDL_main](SDL_main)(). Thus to
ensure that your main() function will not be changed it is necessary to
define [SDL_MAIN_HANDLED](SDL_MAIN_HANDLED) before including SDL.h.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_Init](SDL_Init)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMain](CategoryMain)

