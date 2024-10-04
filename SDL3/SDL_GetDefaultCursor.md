###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetDefaultCursor

Get the default cursor.

## Header File

Defined in [<SDL3/SDL_mouse.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mouse.h)

## Syntax

```c
SDL_Cursor * SDL_GetDefaultCursor(void);
```

## Return Value

([SDL_Cursor](SDL_Cursor) *) Returns the default cursor on success or NULL
on failuree; call [SDL_GetError](SDL_GetError)() for more information.

## Remarks

You do not have to call [SDL_DestroyCursor](SDL_DestroyCursor)() on the
return value, but it is safe to do so.

## Version

This function is available since SDL 3.0.0.

## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMouse](CategoryMouse)

