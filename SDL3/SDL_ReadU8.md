###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_ReadU8

Use this function to read a byte from an [SDL_IOStream](SDL_IOStream).

## Header File

Defined in [<SDL3/SDL_iostream.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_iostream.h)

## Syntax

```c
bool SDL_ReadU8(SDL_IOStream *src, Uint8 *value);
```

## Function Parameters

|                                |           |                                                |
| ------------------------------ | --------- | ---------------------------------------------- |
| [SDL_IOStream](SDL_IOStream) * | **src**   | the [SDL_IOStream](SDL_IOStream) to read from. |
| Uint8 *                        | **value** | a pointer filled in with the data read.        |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.0.0.

## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryIOStream](CategoryIOStream)

