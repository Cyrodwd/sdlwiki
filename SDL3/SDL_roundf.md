###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_roundf

Round `x` to the nearest integer.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
float SDL_roundf(float x);
```

## Function Parameters

|       |       |                       |
| ----- | ----- | --------------------- |
| float | **x** | floating point value. |

## Return Value

(float) Returns the nearest integer to `x`.

## Remarks

Rounds `x` to the nearest integer. Values halfway between integers will be
rounded away from zero.

Domain: `-INF <= x <= INF`

Range: `-INF <= y <= INF`, y integer

This function operates on double-precision floating point values, use
[SDL_roundf](SDL_roundf) for single-precision floats. To get the result as
an integer type, use [SDL_lroundf](SDL_lroundf).

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_round](SDL_round)
- [SDL_lroundf](SDL_lroundf)
- [SDL_floorf](SDL_floorf)
- [SDL_ceilf](SDL_ceilf)
- [SDL_truncf](SDL_truncf)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

