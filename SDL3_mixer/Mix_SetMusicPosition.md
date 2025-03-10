###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_SetMusicPosition

Set the current position in the music stream, in seconds.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_SetMusicPosition(double position);
```

## Function Parameters

|        |              |                                             |
| ------ | ------------ | ------------------------------------------- |
| double | **position** | the new position, in seconds (as a double). |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information.

## Remarks

To convert from milliseconds, divide by 1000.0.

This function is only implemented for MOD music formats (set pattern order
number) and for WAV, OGG, FLAC, MP3, and MOD music at the moment.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

