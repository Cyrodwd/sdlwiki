###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_FadeInMusic

Play a new music object, fading in the audio.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_FadeInMusic(Mix_Music *music, int loops, int ms);
```

## Function Parameters

|                          |           |                                                                                  |
| ------------------------ | --------- | -------------------------------------------------------------------------------- |
| [Mix_Music](Mix_Music) * | **music** | the new music object to play.                                                    |
| int                      | **loops** | the number of times the chunk should loop, -1 to loop (not actually) infinitely. |
| int                      | **ms**    | the number of milliseconds to spend fading in.                                   |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information.

## Remarks

This will start the new music playing, much like
[Mix_PlayMusic](Mix_PlayMusic)() will, but will start the music playing at
silence and fade in to its normal volume over the specified number of
milliseconds.

If there is already music playing, that music will be halted and the new
music object will take its place.

If `loops` is greater than zero, loop the music that many times. If `loops`
is -1, loop "infinitely" (~65000 times).

Fading music will change it's volume progressively, as if
[Mix_VolumeMusic](Mix_VolumeMusic)() was called on it (which is to say: you
probably shouldn't call [Mix_VolumeMusic](Mix_VolumeMusic)() on fading
music).

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

