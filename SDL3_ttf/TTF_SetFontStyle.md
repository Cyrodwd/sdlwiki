###### (This function is part of SDL_ttf, a separate library from SDL.)
# TTF_SetFontStyle

Set a font's current style.

## Header File

Defined in [<SDL3_ttf/SDL_ttf.h>](https://github.com/libsdl-org/SDL_ttf/blob/main/include/SDL3_ttf/SDL_ttf.h)

## Syntax

```c
void TTF_SetFontStyle(TTF_Font *font, int style);
```

## Function Parameters

|                        |           |                                             |
| ---------------------- | --------- | ------------------------------------------- |
| [TTF_Font](TTF_Font) * | **font**  | the font to set a new style on.             |
| int                    | **style** | the new style values to set, OR'd together. |

## Remarks

This clears already-generated glyphs, if any, from the cache.

The font styles are a set of bit flags, OR'd together:

- [`TTF_STYLE_NORMAL`](TTF_STYLE_NORMAL) (is zero)
- [`TTF_STYLE_BOLD`](TTF_STYLE_BOLD)
- [`TTF_STYLE_ITALIC`](TTF_STYLE_ITALIC)
- [`TTF_STYLE_UNDERLINE`](TTF_STYLE_UNDERLINE)
- [`TTF_STYLE_STRIKETHROUGH`](TTF_STYLE_STRIKETHROUGH)

## Thread Safety

This function should be called on the thread that created the font.

## Version

This function is available since SDL_ttf 3.0.0.

## See Also

- [TTF_GetFontStyle](TTF_GetFontStyle)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

