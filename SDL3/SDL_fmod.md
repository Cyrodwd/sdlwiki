# SDL_fmod

Return the floating-point remainder of `x / y`

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
double SDL_fmod(double x, double y);
```

## Function Parameters

|        |       |                                 |
| ------ | ----- | ------------------------------- |
| double | **x** | the numerator.                  |
| double | **y** | the denominator. Must not be 0. |

## Return Value

(double) Returns the remainder of `x / y`.

## Remarks

Divides `x` by `y`, and returns the remainder.

Domain: `-INF <= x <= INF`, `-INF <= y <= INF`, `y != 0`

Range: `-y <= z <= y`

This function operates on double-precision floating point values, use
[SDL_fmodf](SDL_fmodf) for single-precision floats.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_fmodf](SDL_fmodf)
- [SDL_modf](SDL_modf)
- [SDL_trunc](SDL_trunc)
- [SDL_ceil](SDL_ceil)
- [SDL_floor](SDL_floor)
- [SDL_round](SDL_round)
- [SDL_lround](SDL_lround)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

