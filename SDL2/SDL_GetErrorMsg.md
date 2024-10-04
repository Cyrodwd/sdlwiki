###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetErrorMsg

Get the last error message that was set for the current thread.

## Header File

Defined in [SDL_error.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_error.h)

## Syntax

```c
char * SDL_GetErrorMsg(char *errstr, int maxlen);
```

## Function Parameters

|        |            |                                                                                   |
| ------ | ---------- | --------------------------------------------------------------------------------- |
| char * | **errstr** | A buffer to fill with the last error message that was set for the current thread. |
| int    | **maxlen** | The size of the buffer pointed to by the errstr parameter.                        |

## Return Value

(char *) Returns the pointer passed in as the `errstr` parameter.

## Remarks

This allows the caller to copy the error string into a provided buffer, but
otherwise operates exactly the same as [SDL_GetError](SDL_GetError)().

## Version

This function is available since SDL 2.0.14.

## See Also

- [SDL_GetError](SDL_GetError)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryError](CategoryError)

