###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_RWFromConstMem

Use this function to prepare a read-only memory buffer for use with RWops.

## Header File

Defined in [SDL_rwops.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rwops.h)

## Syntax

```c
SDL_RWops* SDL_RWFromConstMem(const void *mem,
                              int size);
```

## Function Parameters

|              |          |                                                                           |
| ------------ | -------- | ------------------------------------------------------------------------- |
| const void * | **mem**  | a pointer to a read-only buffer to feed an [SDL_RWops](SDL_RWops) stream. |
| int          | **size** | the buffer size, in bytes.                                                |

## Return Value

([SDL_RWops](SDL_RWops) *) Returns a pointer to a new
[SDL_RWops](SDL_RWops) structure, or NULL if it fails; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function sets up an [SDL_RWops](SDL_RWops) struct based on a memory
area of a certain size. It assumes the memory area is not writable.

Attempting to write to this RWops stream will report an error without
writing to the memory buffer.

This memory buffer is not copied by the RWops; the pointer you provide must
remain valid until you close the stream. Closing the stream will not free
the original buffer.

If you need to write to a memory buffer, you should use
[SDL_RWFromMem](SDL_RWFromMem)() with a writable buffer of memory instead.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_RWclose](SDL_RWclose)
- [SDL_RWFromConstMem](SDL_RWFromConstMem)
- [SDL_RWFromFile](SDL_RWFromFile)
- [SDL_RWFromFP](SDL_RWFromFP)
- [SDL_RWFromMem](SDL_RWFromMem)
- [SDL_RWread](SDL_RWread)
- [SDL_RWseek](SDL_RWseek)
- [SDL_RWtell](SDL_RWtell)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRWOPS](CategoryRWOPS)

