###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_ClearHints

Clear all hints.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
void SDL_ClearHints(void);
```

## Remarks

This function is automatically called during [SDL_Quit](SDL_Quit)(), and
deletes all callbacks without calling them and frees all memory associated
with hints. If you're calling this from application code you probably want
to call [SDL_ResetHints](SDL_ResetHints)() instead.

This function will be removed from the API the next time we rev the ABI.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_ResetHints](SDL_ResetHints)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHints](CategoryHints)

