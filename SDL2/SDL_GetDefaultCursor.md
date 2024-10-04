###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetDefaultCursor

Get the default cursor.

## Header File

Defined in [SDL_mouse.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_mouse.h)

## Syntax

```c
SDL_Cursor* SDL_GetDefaultCursor(void);
```

## Return Value

([SDL_Cursor](SDL_Cursor) *) Returns the default cursor on success or NULL
on failure.

## Remarks

You do not have to call [SDL_FreeCursor](SDL_FreeCursor)() on the return
value, but it is safe to do so.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_CreateSystemCursor](SDL_CreateSystemCursor)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMouse](CategoryMouse)

