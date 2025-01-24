# SDL_islower

Report if a character is lower case.

## Header File

Defined in [<SDL3/SDL_stdinc.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_stdinc.h)

## Syntax

```c
int SDL_islower(int x);
```

## Function Parameters

|     |       |                           |
| --- | ----- | ------------------------- |
| int | **x** | character value to check. |

## Return Value

(int) Returns non-zero if x falls within the character class, zero
otherwise.

## Remarks

**WARNING**: Regardless of system locale, this will only treat ASCII values
'a' through 'z' as true.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdinc](CategoryStdinc)

