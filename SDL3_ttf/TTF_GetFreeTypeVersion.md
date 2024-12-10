###### (This function is part of SDL_ttf, a separate library from SDL.)
# TTF_GetFreeTypeVersion

Query the version of the FreeType library in use.

## Header File

Defined in [<SDL3_ttf/SDL_ttf.h>](https://github.com/libsdl-org/SDL_ttf/blob/main/include/SDL3_ttf/SDL_ttf.h)

## Syntax

```c
void TTF_GetFreeTypeVersion(int *major, int *minor, int *patch);
```

## Function Parameters

|       |           |                                                             |
| ----- | --------- | ----------------------------------------------------------- |
| int * | **major** | to be filled in with the major version number. Can be NULL. |
| int * | **minor** | to be filled in with the minor version number. Can be NULL. |
| int * | **patch** | to be filled in with the param version number. Can be NULL. |

## Remarks

[TTF_Init](TTF_Init)() should be called before calling this function.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL_ttf 3.0.0.

## See Also

- [TTF_Init](TTF_Init)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLTTF](CategorySDLTTF)

