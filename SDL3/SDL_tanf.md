###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_tanf

Compute the tangent of `x`.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
float SDL_tanf(float x);
```

## Function Parameters

|       |       |                                   |
| ----- | ----- | --------------------------------- |
| float | **x** | floating point value, in radians. |

## Return Value

(float) Returns tangent of `x`.

## Remarks

Domain: `-INF <= x <= INF`

Range: `-INF <= y <= INF`

This function operates on single-precision floating point values, use
[SDL_tanf](SDL_tanf) for double-precision floats.

This function may use a different approximation across different versions,
platforms and configurations. i.e, it can return a different value given
the same input on different machines or operating systems, or if SDL is
updated.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_tan](SDL_tan)
- [SDL_sinf](SDL_sinf)
- [SDL_cosf](SDL_cosf)
- [SDL_atanf](SDL_atanf)
- [SDL_atan2f](SDL_atan2f)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

