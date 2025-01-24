# SDL_fabs

Compute the absolute value of `x`

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
double SDL_fabs(double x);
```

## Function Parameters

|        |       |                                               |
| ------ | ----- | --------------------------------------------- |
| double | **x** | floating point value to use as the magnitude. |

## Return Value

(double) Returns the absolute value of `x`.

## Remarks

Domain: `-INF <= x <= INF`

Range: `0 <= y <= INF`

This function operates on double-precision floating point values, use
[SDL_copysignf](SDL_copysignf) for single-precision floats.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_fabsf](SDL_fabsf)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

