###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_WinRTGetFSPathUNICODE

Retrieve a WinRT defined path on the local file system.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
const wchar_t * SDL_WinRTGetFSPathUNICODE(SDL_WinRT_Path pathType);
```

## Function Parameters

|                                  |              |                                                                        |
| -------------------------------- | ------------ | ---------------------------------------------------------------------- |
| [SDL_WinRT_Path](SDL_WinRT_Path) | **pathType** | the type of path to retrieve, one of [SDL_WinRT_Path](SDL_WinRT_Path). |

## Return Value

(const wchar_t *) Returns a UCS-2 string (16-bit, wide-char) containing the
path, or NULL if the path is not available for any reason; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Not all paths are available on all versions of Windows. This is especially
true on Windows Phone. Check the documentation for the given
[SDL_WinRT_Path](SDL_WinRT_Path) for more information on which path types
are supported where.

Documentation on most app-specific path types on WinRT can be found on
MSDN, at the URL:

https://msdn.microsoft.com/en-us/library/windows/apps/hh464917.aspx

## Version

This function is available since SDL 2.0.3.

## See Also

- [SDL_WinRTGetFSPathUTF8](SDL_WinRTGetFSPathUTF8)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

