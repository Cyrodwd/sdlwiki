# SDL_Metal_CreateView

Create a CAMetalLayer-backed NSView/UIView and attach it to the specified window.

## Header File

Defined in [SDL_metal.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_metal.h)

## Syntax

```c
SDL_MetalView SDL_Metal_CreateView(SDL_Window * window);
```

## Remarks

On macOS, this does *not* associate a MTLDevice with the CAMetalLayer on
its own. It is up to user code to do that.

The returned handle can be casted directly to a NSView or UIView. To access
the backing CAMetalLayer, call [SDL_Metal_GetLayer](SDL_Metal_GetLayer)().

## Version

This function is available since SDL 2.0.12.

## See Also

- [SDL_Metal_DestroyView](SDL_Metal_DestroyView)
- [SDL_Metal_GetLayer](SDL_Metal_GetLayer)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMetal](CategoryMetal)

