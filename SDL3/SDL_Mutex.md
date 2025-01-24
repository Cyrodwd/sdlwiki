# SDL_Mutex

A means to serialize access to a resource between threads.

## Header File

Defined in [<SDL3/SDL_mutex.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mutex.h)

## Syntax

```c
typedef struct SDL_Mutex SDL_Mutex;
```

## Remarks

Mutexes (short for "mutual exclusion") are a synchronization primitive that
allows exactly one thread to proceed at a time.

Wikipedia has a thorough explanation of the concept:

https://en.wikipedia.org/wiki/Mutex

## Version

This struct is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryMutex](CategoryMutex)

