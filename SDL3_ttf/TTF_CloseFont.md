###### (This function is part of SDL_ttf, a separate library from SDL.)
# TTF_CloseFont

Dispose of a previously-created font.

## Header File

Defined in [<SDL3_ttf/SDL_ttf.h>](https://github.com/libsdl-org/SDL_ttf/blob/main/include/SDL3_ttf/SDL_ttf.h)

## Syntax

```c
void TTF_CloseFont(TTF_Font *font);
```

## Function Parameters

|                        |          |                         |
| ---------------------- | -------- | ----------------------- |
| [TTF_Font](TTF_Font) * | **font** | the font to dispose of. |

## Remarks

Call this when done with a font. This function will free any resources
associated with it. It is safe to call this function on NULL, for example
on the result of a failed call to [TTF_OpenFont](TTF_OpenFont)().

The font is not valid after being passed to this function. String pointers
from functions that return information on this font, such as
[TTF_GetFontFamilyName](TTF_GetFontFamilyName)() and
[TTF_GetFontStyleName](TTF_GetFontStyleName)(), are no longer valid after
this call, as well.

## Thread Safety

This function should not be called while any other thread is using the
font.

## Version

This function is available since SDL_ttf 3.0.0.

## See Also

- [TTF_OpenFont](TTF_OpenFont)
- [TTF_OpenFontIndexDPIIO](TTF_OpenFontIndexDPIIO)
- [TTF_OpenFontIO](TTF_OpenFontIO)
- [TTF_OpenFontDPI](TTF_OpenFontDPI)
- [TTF_OpenFontDPIIO](TTF_OpenFontDPIIO)
- [TTF_OpenFontIndex](TTF_OpenFontIndex)
- [TTF_OpenFontIndexDPI](TTF_OpenFontIndexDPI)
- [TTF_OpenFontIndexDPIIO](TTF_OpenFontIndexDPIIO)
- [TTF_OpenFontIndexIO](TTF_OpenFontIndexIO)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

