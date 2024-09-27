###### (This function is part of SDL_ttf, a separate library from SDL.)
# TTF_GetFontStyle

Query a font's current style.

## Header File

Defined in [<SDL3_ttf/SDL_ttf.h>](https://github.com/libsdl-org/SDL_ttf/blob/main/include/SDL3_ttf/SDL_ttf.h)

## Syntax

```c
int TTF_GetFontStyle(const TTF_Font *font);
```

## Function Parameters

|                              |          |                    |
| ---------------------------- | -------- | ------------------ |
| const [TTF_Font](TTF_Font) * | **font** | the font to query. |

## Return Value

(int) Returns the current font style, as a set of bit flags.

## Remarks

The font styles are a set of bit flags, OR'd together:

- [`TTF_STYLE_NORMAL`](TTF_STYLE_NORMAL) (is zero)
- [`TTF_STYLE_BOLD`](TTF_STYLE_BOLD)
- [`TTF_STYLE_ITALIC`](TTF_STYLE_ITALIC)
- [`TTF_STYLE_UNDERLINE`](TTF_STYLE_UNDERLINE)
- [`TTF_STYLE_STRIKETHROUGH`](TTF_STYLE_STRIKETHROUGH)

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL_ttf 3.0.0.

## See Also

- [TTF_SetFontStyle](TTF_SetFontStyle)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

