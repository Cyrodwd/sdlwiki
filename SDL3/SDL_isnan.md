# SDL_isnan

Return whether the value is NaN.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
int SDL_isnan(double x);
```

## Function Parameters

|        |       |                                        |
| ------ | ----- | -------------------------------------- |
| double | **x** | double-precision floating point value. |

## Return Value

(int) Returns non-zero if the value is NaN, 0 otherwise.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_isnanf](SDL_isnanf)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

