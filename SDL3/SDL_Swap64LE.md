# SDL_Swap64LE

Swap a 64-bit value from littleendian to native byte order.

## Header File

Defined in [<SDL3/SDL_endian.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_endian.h)

## Syntax

```c
#define SDL_Swap64LE(x) SwapOnlyIfNecessary(x)
```

## Macro Parameters

|       |                                                |
| ----- | ---------------------------------------------- |
| **x** | the value to swap, in littleendian byte order. |

## Return Value

Returns `x` in native byte order.

## Remarks

If this is running on a littleendian system, `x` is returned unchanged.

This macro never references `x` more than once, avoiding side effects.

## Thread Safety

It is safe to call this macro from any thread.

## Version

This macro is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryEndian](CategoryEndian)

