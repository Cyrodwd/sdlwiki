# SDL_scalbn

Scale `x` by an integer power of two.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
double SDL_scalbn(double x, int n);
```

## Function Parameters

|        |       |                                    |
| ------ | ----- | ---------------------------------- |
| double | **x** | floating point value to be scaled. |
| int    | **n** | integer exponent.                  |

## Return Value

(double) Returns `x * 2^n`.

## Remarks

Multiplies `x` by the `n`th power of the floating point radix (always 2).

Domain: `-INF <= x <= INF`, `n` integer

Range: `-INF <= y <= INF`

This function operates on double-precision floating point values, use
[SDL_scalbnf](SDL_scalbnf) for single-precision floats.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_scalbnf](SDL_scalbnf)
- [SDL_pow](SDL_pow)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

