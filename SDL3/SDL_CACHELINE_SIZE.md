# SDL_CACHELINE_SIZE

A guess for the cacheline size used for padding.

## Header File

Defined in [<SDL3/SDL_cpuinfo.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_cpuinfo.h)

## Syntax

```c
#define SDL_CACHELINE_SIZE  128
```

## Remarks

Most x86 processors have a 64 byte cache line. The 64-bit PowerPC
processors have a 128 byte cache line. We use the larger value to be
generally safe.

## Version

This macro is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryCPUInfo](CategoryCPUInfo)

