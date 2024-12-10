###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_EachSoundFont

Iterate SoundFonts paths to use by supported MIDI backends.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_EachSoundFont(Mix_EachSoundFontCallback function, void *data);
```

## Function Parameters

|                                                        |              |                                                             |
| ------------------------------------------------------ | ------------ | ----------------------------------------------------------- |
| [Mix_EachSoundFontCallback](Mix_EachSoundFontCallback) | **function** | the callback function to call once per path.                |
| void *                                                 | **data**     | a pointer to pass to the callback for its own personal use. |

## Return Value

(bool) Returns true if callback ever returned true, false on error or if
the callback never returned true.

## Remarks

This function will take the string reported by
[Mix_GetSoundFonts](Mix_GetSoundFonts)(), split it up into separate paths,
as delimited by semicolons in the string, and call a callback function for
each separate path.

If there are no paths available, this returns 0 without calling the
callback at all.

If the callback returns non-zero, this function stops iterating and returns
non-zero. If the callback returns 0, this function will continue iterating,
calling the callback again for further paths. If the callback never returns
1, this function returns 0, so this can be used to decide if an available
soundfont is acceptable for use.

## Version

This function is available since SDL_mixer 3.0.0.

## See Also

- [Mix_GetSoundFonts](Mix_GetSoundFonts)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

