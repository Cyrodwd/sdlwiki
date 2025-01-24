# SDL_tolower

Convert low-ASCII English letters to lowercase.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
int SDL_tolower(int x);
```

## Function Parameters

|     |       |                           |
| --- | ----- | ------------------------- |
| int | **x** | character value to check. |

## Return Value

(int) Returns lowercase version of x, or x if no conversion available.

## Remarks

**WARNING**: Regardless of system locale, this will only convert ASCII
values 'A' through 'Z' to lowercase.

This function returns the lowercase equivalent of `x`. If a character
cannot be converted, or is already lowercase, this function returns `x`.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

