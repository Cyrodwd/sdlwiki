# SDL_WriteLE64

Use this function to write 64 bits in native format to a [SDL_RWops](SDL_RWops) as little-endian data.

## Header File

Defined in [SDL_rwops.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rwops.h)

## Syntax

```c
size_t SDL_WriteLE64(SDL_RWops * dst, Uint64 value);
```

## Function Parameters

|                          |           |                                           |
| ------------------------ | --------- | ----------------------------------------- |
| [SDL_RWops](SDL_RWops) * | **dst**   | the stream to which data will be written. |
| [Uint64](Uint64)         | **value** | the data to be written, in native format. |

## Return Value

(size_t) Returns 1 on successful write, 0 on error.

## Remarks

SDL byteswaps the data only if necessary, so the application always
specifies native format, and the data written will be in little-endian
format.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_WriteBE64](SDL_WriteBE64)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRWOPS](CategoryRWOPS)

