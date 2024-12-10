###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_GetMusicVolume

Query the current volume value for a music object.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
int Mix_GetMusicVolume(Mix_Music *music);
```

## Function Parameters

|                          |           |                            |
| ------------------------ | --------- | -------------------------- |
| [Mix_Music](Mix_Music) * | **music** | the music object to query. |

## Return Value

(int) Returns the music's current volume, between 0 and
[MIX_MAX_VOLUME](MIX_MAX_VOLUME) (128).

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

