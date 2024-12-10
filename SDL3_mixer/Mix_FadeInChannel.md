###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_FadeInChannel

Play an audio chunk on a specific channel, fading in the audio.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
int Mix_FadeInChannel(int channel, Mix_Chunk *chunk, int loops, int ms);
```

## Function Parameters

|                          |             |                                                                                  |
| ------------------------ | ----------- | -------------------------------------------------------------------------------- |
| int                      | **channel** | the channel on which to play the new chunk, or -1 to find any available.         |
| [Mix_Chunk](Mix_Chunk) * | **chunk**   | the new chunk to play.                                                           |
| int                      | **loops**   | the number of times the chunk should loop, -1 to loop (not actually) infinitely. |
| int                      | **ms**      | the number of milliseconds to spend fading in.                                   |

## Return Value

(int) Returns which channel was used to play the sound, or -1 if sound
could not be played.

## Remarks

This will start the new sound playing, much like
[Mix_PlayChannel](Mix_PlayChannel)() will, but will start the sound playing
at silence and fade in to its normal volume over the specified number of
milliseconds.

If the specified channel is -1, play on the first free channel (and return
-1 without playing anything new if no free channel was available).

If a specific channel was requested, and there is a chunk already playing
there, that chunk will be halted and the new chunk will take its place.

If `loops` is greater than zero, loop the sound that many times. If `loops`
is -1, loop "infinitely" (~65000 times).

A fading channel will change it's volume progressively, as if
[Mix_Volume](Mix_Volume)() was called on it (which is to say: you probably
shouldn't call [Mix_Volume](Mix_Volume)() on a fading channel).

Note that before SDL_mixer 3.0.0, this function was a macro that called
[Mix_FadeInChannelTimed](Mix_FadeInChannelTimed)() with a fourth parameter
("ticks") of -1. This function still does the same thing, but promotes it
to a proper API function. Older binaries linked against a newer SDL_mixer
will still call [Mix_FadeInChannelTimed](Mix_FadeInChannelTimed) directly,
as they are using the macro, which was available since the dawn of time.

## Version

This function is available since SDL_mixer 3.0.0

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

