###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetRevision

Get the code revision of SDL that is linked against your program.

## Header File

Defined in [SDL_version.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_version.h)

## Syntax

```c
const char* SDL_GetRevision(void);
```

## Return Value

(const char *) Returns an arbitrary string, uniquely identifying the exact
revision of the SDL library in use.

## Remarks

This value is the revision of the code you are linked with and may be
different from the code you are compiling with, which is found in the
constant [SDL_REVISION](SDL_REVISION).

The revision is arbitrary string (a hash value) uniquely identifying the
exact revision of the SDL library in use, and is only useful in comparing
against other revisions. It is NOT an incrementing number.

If SDL wasn't built from a git repository with the appropriate tools, this
will return an empty string.

Prior to SDL 2.0.16, before development moved to GitHub, this returned a
hash for a Mercurial repository.

You shouldn't use this function for anything but logging it for debugging
purposes. The string is not intended to be reliable in any way.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetVersion](SDL_GetVersion)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVersion](CategoryVersion)

