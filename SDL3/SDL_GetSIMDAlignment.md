# SDL_GetSIMDAlignment

Report the alignment this system needs for SIMD allocations.

## Header File

Defined in [<SDL3/SDL_cpuinfo.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_cpuinfo.h)

## Syntax

```c
size_t SDL_GetSIMDAlignment(void);
```

## Return Value

(size_t) Returns the alignment in bytes needed for available, known SIMD
instructions.

## Remarks

This will return the minimum number of bytes to which a pointer must be
aligned to be compatible with SIMD instructions on the current machine. For
example, if the machine supports SSE only, it will return 16, but if it
supports AVX-512F, it'll return 64 (etc). This only reports values for
instruction sets SDL knows about, so if your SDL build doesn't have
[SDL_HasAVX512F](SDL_HasAVX512F)(), then it might return 16 for the SSE
support it sees and not 64 for the AVX-512 instructions that exist but SDL
doesn't know about. Plan accordingly.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_aligned_alloc](SDL_aligned_alloc)
- [SDL_aligned_free](SDL_aligned_free)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryCPUInfo](CategoryCPUInfo)

