###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_Condition

A means to block multiple threads until a condition is satisfied.

## Header File

Defined in [<SDL3/SDL_mutex.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mutex.h)

## Syntax

```c
typedef struct SDL_Condition SDL_Condition;
```

## Remarks

Condition variables, paired with an [SDL_Mutex](SDL_Mutex), let an app halt
multiple threads until a condition has occurred, at which time the app can
release one or all waiting threads.

Wikipedia has a thorough explanation of the concept:

https://en.wikipedia.org/wiki/Condition_variable

## Version

This struct is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryMutex](CategoryMutex)

