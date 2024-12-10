###### (This function is part of SDL_ttf, a separate library from SDL.)
# SDL_TTF_VERSION_ATLEAST

This macro will evaluate to true if compiled with SDL_ttf at least X.Y.Z.

## Header File

Defined in [<SDL3_ttf/SDL_ttf.h>](https://github.com/libsdl-org/SDL_ttf/blob/main/include/SDL3_ttf/SDL_ttf.h)

## Syntax

```c
#define SDL_TTF_VERSION_ATLEAST(X, Y, Z) \
    ((SDL_TTF_MAJOR_VERSION >= X) && \
     (SDL_TTF_MAJOR_VERSION > X || SDL_TTF_MINOR_VERSION >= Y) && \
     (SDL_TTF_MAJOR_VERSION > X || SDL_TTF_MINOR_VERSION > Y || SDL_TTF_MICRO_VERSION >= Z))
```

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategorySDLTTF](CategorySDLTTF)

