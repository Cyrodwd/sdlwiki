###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_cosf

Compute the cosine of `x`.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
float SDL_cosf(float x);
```

## Function Parameters

|       |       |                                   |
| ----- | ----- | --------------------------------- |
| float | **x** | floating point value, in radians. |

## Return Value

(float) Returns cosine of `x`.

## Remarks

Domain: `-INF <= x <= INF`

Range: `-1 <= y <= 1`

This function operates on single-precision floating point values, use
[SDL_cos](SDL_cos) for double-precision floats.

This function may use a different approximation across different versions,
platforms and configurations. i.e, it can return a different value given
the same input on different machines or operating systems, or if SDL is
updated.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_cos](SDL_cos)
- [SDL_acosf](SDL_acosf)
- [SDL_sinf](SDL_sinf)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

