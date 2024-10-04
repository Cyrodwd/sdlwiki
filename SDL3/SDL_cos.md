###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_cos

Compute the cosine of `x`.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
double SDL_cos(double x);
```

## Function Parameters

|        |       |                                   |
| ------ | ----- | --------------------------------- |
| double | **x** | floating point value, in radians. |

## Return Value

(double) Returns cosine of `x`.

## Remarks

Domain: `-INF <= x <= INF`

Range: `-1 <= y <= 1`

This function operates on double-precision floating point values, use
[SDL_cosf](SDL_cosf) for single-precision floats.

This function may use a different approximation across different versions,
platforms and configurations. i.e, it can return a different value given
the same input on different machines or operating systems, or if SDL is
updated.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_cosf](SDL_cosf)
- [SDL_acos](SDL_acos)
- [SDL_sin](SDL_sin)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

