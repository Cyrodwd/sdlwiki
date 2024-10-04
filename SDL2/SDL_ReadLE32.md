###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_ReadLE32

Use this function to read 32 bits of little-endian data from an [SDL_RWops](SDL_RWops) and return in native format.

## Header File

Defined in [SDL_rwops.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rwops.h)

## Syntax

```c
Uint32 SDL_ReadLE32(SDL_RWops * src);
```

## Function Parameters

|                          |         |                                     |
| ------------------------ | ------- | ----------------------------------- |
| [SDL_RWops](SDL_RWops) * | **src** | the stream from which to read data. |

## Return Value

(Uint32) Returns 32 bits of data in the native byte order of the platform.

## Remarks

SDL byteswaps the data only if necessary, so the data returned will be in
the native byte order.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_ReadBE32](SDL_ReadBE32)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRWOPS](CategoryRWOPS)

