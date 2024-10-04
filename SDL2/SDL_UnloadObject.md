###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_UnloadObject

Unload a shared object from memory.

## Header File

Defined in [SDL_loadso.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_loadso.h)

## Syntax

```c
void SDL_UnloadObject(void *handle);
```

## Function Parameters

|        |            |                                                                              |
| ------ | ---------- | ---------------------------------------------------------------------------- |
| void * | **handle** | a valid shared object handle returned by [SDL_LoadObject](SDL_LoadObject)(). |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_LoadFunction](SDL_LoadFunction)
- [SDL_LoadObject](SDL_LoadObject)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryLoadSO](CategoryLoadSO)

