# SDL_LoadFile

Load all the data from a file path.

## Header File

Defined in [SDL_rwops.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rwops.h)

## Syntax

```c
void* SDL_LoadFile(const char *file, size_t *datasize);
```

## Function Parameters

|              |              |                                                   |
| ------------ | ------------ | ------------------------------------------------- |
| const char * | **file**     | the path to read all available data from.         |
| size_t *     | **datasize** | if not NULL, will store the number of bytes read. |

## Return Value

(void *) Returns the data, or NULL if there was an error.

## Remarks

The data is allocated with a zero byte at the end (null terminated) for
convenience. This extra byte is not included in the value reported via
`datasize`.

The data should be freed with [SDL_free](SDL_free)().

Prior to SDL 2.0.10, this function was a macro wrapping around
[SDL_LoadFile_RW](SDL_LoadFile_RW).

## Version

This function is available since SDL 2.0.10.

## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRWOPS](CategoryRWOPS)

