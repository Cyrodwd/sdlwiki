###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_GetMusicTitle

Get the title for a music object, or its filename.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
const char* Mix_GetMusicTitle(const Mix_Music *music);
```

## Function Parameters

|                                |           |                                                                     |
| ------------------------------ | --------- | ------------------------------------------------------------------- |
| const [Mix_Music](Mix_Music) * | **music** | the music object to query, or NULL for the currently-playing music. |

## Return Value

(const char *) Returns the music's title if available, or the filename if
not, or "".

## Remarks

This returns format-specific metadata. Not all file formats supply this!

If `music` is NULL, this will query the currently-playing music.

If music's title tag is missing or empty, the filename will be returned. If
you'd rather have the actual metadata or nothing, use
[Mix_GetMusicTitleTag](Mix_GetMusicTitleTag)() instead.

Please note that if the music was loaded from an SDL_IOStream instead of a
filename, the filename returned will be an empty string ("").

This function never returns NULL! If no data is available, it will return
an empty string ("").

## Version

This function is available since SDL_mixer 3.0.0.

## See Also

- [Mix_GetMusicTitleTag](Mix_GetMusicTitleTag)
- [Mix_GetMusicArtistTag](Mix_GetMusicArtistTag)
- [Mix_GetMusicAlbumTag](Mix_GetMusicAlbumTag)
- [Mix_GetMusicCopyrightTag](Mix_GetMusicCopyrightTag)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

