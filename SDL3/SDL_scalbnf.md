###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_scalbnf

Scale `x` by an integer power of two.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
float SDL_scalbnf(float x, int n);
```

## Function Parameters

|       |       |                                    |
| ----- | ----- | ---------------------------------- |
| float | **x** | floating point value to be scaled. |
| int   | **n** | integer exponent.                  |

## Return Value

(float) Returns `x * 2^n`.

## Remarks

Multiplies `x` by the `n`th power of the floating point radix (always 2).

Domain: `-INF <= x <= INF`, `n` integer

Range: `-INF <= y <= INF`

This function operates on single-precision floating point values, use
[SDL_scalbn](SDL_scalbn) for double-precision floats.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_scalbn](SDL_scalbn)
- [SDL_powf](SDL_powf)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

