# SDL_iconv_string

This function converts a buffer or string between encodings in one pass, returning a string that must be freed with [SDL_free](SDL_free)() or NULL on error.

## Header File

Defined in [SDL_stdinc.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_stdinc.h)

## Syntax

```c
char* SDL_iconv_string(const char *tocode,
                       const char *fromcode,
                       const char *inbuf,
                       size_t inbytesleft);
```

## Version

This function is available since SDL 2.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStdInc](CategoryStdInc)

