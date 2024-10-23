###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_TimeToWindows

Converts an SDL time into a Windows FILETIME (100-nanosecond intervals since January 1, 1601).

## Header File

Defined in [<SDL3/SDL_time.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_time.h)

## Syntax

```c
void SDL_TimeToWindows(SDL_Time ticks, Uint32 *dwLowDateTime, Uint32 *dwHighDateTime);
```

## Function Parameters

|                      |                    |                                                                          |
| -------------------- | ------------------ | ------------------------------------------------------------------------ |
| [SDL_Time](SDL_Time) | **ticks**          | the time to convert.                                                     |
| Uint32 *             | **dwLowDateTime**  | a pointer filled in with the low portion of the Windows FILETIME value.  |
| Uint32 *             | **dwHighDateTime** | a pointer filled in with the high portion of the Windows FILETIME value. |

## Remarks

This function fills in the two 32-bit values of the FILETIME structure.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryTime](CategoryTime)

