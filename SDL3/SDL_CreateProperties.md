# SDL_CreateProperties

Create a group of properties.

## Header File

Defined in [<SDL3/SDL_properties.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_properties.h)

## Syntax

```c
SDL_PropertiesID SDL_CreateProperties(void);
```

## Return Value

([SDL_PropertiesID](SDL_PropertiesID)) Returns an ID for a new group of
properties, or 0 on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

All properties are automatically destroyed when [SDL_Quit](SDL_Quit)() is
called.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_DestroyProperties](SDL_DestroyProperties)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryProperties](CategoryProperties)

