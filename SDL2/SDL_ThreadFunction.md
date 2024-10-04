###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_ThreadFunction

The function passed to [SDL_CreateThread](SDL_CreateThread)().

## Header File

Defined in [SDL_thread.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_thread.h)

## Syntax

```c
typedef int (SDLCALL * SDL_ThreadFunction) (void *data);
```

## Function Parameters

|          |                                                                      |
| -------- | -------------------------------------------------------------------- |
| **data** | what was passed as `data` to [SDL_CreateThread](SDL_CreateThread)(). |

## Return Value

Returns a value that can be reported through
[SDL_WaitThread](SDL_WaitThread)().

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIDatatype](CategoryAPIDatatype), [CategoryThread](CategoryThread)

