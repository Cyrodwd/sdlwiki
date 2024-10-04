###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_HasAVX2

Determine whether the CPU has AVX2 features.

## Header File

Defined in [SDL_cpuinfo.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_cpuinfo.h)

## Syntax

```c
SDL_bool SDL_HasAVX2(void);
```

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if the CPU has AVX2
features or [SDL_FALSE](SDL_FALSE) if not.

## Remarks

This always returns false on CPUs that aren't using Intel instruction sets.

## Version

This function is available since SDL 2.0.4.

## See Also

- [SDL_Has3DNow](SDL_Has3DNow)
- [SDL_HasAltiVec](SDL_HasAltiVec)
- [SDL_HasAVX](SDL_HasAVX)
- [SDL_HasMMX](SDL_HasMMX)
- [SDL_HasRDTSC](SDL_HasRDTSC)
- [SDL_HasSSE](SDL_HasSSE)
- [SDL_HasSSE2](SDL_HasSSE2)
- [SDL_HasSSE3](SDL_HasSSE3)
- [SDL_HasSSE41](SDL_HasSSE41)
- [SDL_HasSSE42](SDL_HasSSE42)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryCPUInfo](CategoryCPUInfo)

