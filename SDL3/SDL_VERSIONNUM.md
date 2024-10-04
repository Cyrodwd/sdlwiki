###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_VERSIONNUM

This macro turns the version numbers into a numeric value.

## Header File

Defined in [<SDL3/SDL_version.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_version.h)

## Syntax

```c
#define SDL_VERSIONNUM(major, minor, patch) \
    ((major) * 1000000 + (minor) * 1000 + (patch))
```

## Macro Parameters

|           |                           |
| --------- | ------------------------- |
| **major** | the major version number. |
| **minor** | the minorversion number.  |
| **patch** | the patch version number. |

## Remarks

(1,2,3) becomes 1002003.

## Version

This macro is available since SDL 3.0.0.

## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryVersion](CategoryVersion)

