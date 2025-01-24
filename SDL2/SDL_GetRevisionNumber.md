# SDL_GetRevisionNumber

Obsolete function, do not use.

## Deprecated

Use [SDL_GetRevision](SDL_GetRevision)() instead; if SDL was carefully
built, it will return a git hash.

## Header File

Defined in [SDL_version.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_version.h)

## Syntax

```c
int SDL_GetRevisionNumber(void);
```

## Return Value

(int) Returns zero, always, in modern SDL releases.

## Remarks

When SDL was hosted in a Mercurial repository, and was built carefully,
this would return the revision number that the build was created from. This
number was not reliable for several reasons, but more importantly, SDL is
now hosted in a git repository, which does not offer numbers at all, only
hashes. This function only ever returns zero now. Don't use it.

Before SDL 2.0.16, this might have returned an unreliable, but non-zero
number.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetRevision](SDL_GetRevision)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryVersion](CategoryVersion)

