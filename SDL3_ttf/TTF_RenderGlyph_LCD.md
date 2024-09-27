###### (This function is part of SDL_ttf, a separate library from SDL.)
# TTF_RenderGlyph_LCD

Render a single 32-bit glyph at LCD subpixel quality to a new ARGB surface.

## Header File

Defined in [<SDL3_ttf/SDL_ttf.h>](https://github.com/libsdl-org/SDL_ttf/blob/main/include/SDL3_ttf/SDL_ttf.h)

## Syntax

```c
SDL_Surface * TTF_RenderGlyph_LCD(TTF_Font *font, Uint32 ch, SDL_Color fg, SDL_Color bg);
```

## Function Parameters

|                        |          |                                    |
| ---------------------- | -------- | ---------------------------------- |
| [TTF_Font](TTF_Font) * | **font** | the font to render with.           |
| Uint32                 | **ch**   | the character to render.           |
| SDL_Color              | **fg**   | the foreground color for the text. |
| SDL_Color              | **bg**   | the background color for the text. |

## Return Value

(SDL_Surface *) Returns a new 32-bit, ARGB surface, or NULL if there was an
error.

## Remarks

This function will allocate a new 32-bit, ARGB surface, and render
alpha-blended text using FreeType's LCD subpixel rendering. This function
returns the new surface, or NULL if there was an error.

The glyph is rendered without any padding or centering in the X direction,
and aligned normally in the Y direction.

You can render at other quality levels with
[TTF_RenderGlyph_Solid](TTF_RenderGlyph_Solid),
[TTF_RenderGlyph_Shaded](TTF_RenderGlyph_Shaded), and
[TTF_RenderGlyph_Blended](TTF_RenderGlyph_Blended).

## Thread Safety

This function should be called on the thread that created the font.

## Version

This function is available since SDL_ttf 3.0.0.

## See Also

- [TTF_RenderGlyph_Blended](TTF_RenderGlyph_Blended)
- [TTF_RenderGlyph_Shaded](TTF_RenderGlyph_Shaded)
- [TTF_RenderGlyph_Solid](TTF_RenderGlyph_Solid)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction)

