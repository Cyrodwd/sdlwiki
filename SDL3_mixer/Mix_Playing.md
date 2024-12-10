###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_Playing

Check the playing status of a specific channel.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
int Mix_Playing(int channel);
```

## Function Parameters

|     |             |          |
| --- | ----------- | -------- |
| int | **channel** | channel. |

## Return Value

(int) Returns non-zero if channel is playing, zero otherwise. If `channel`
is -1, return the total number of channel playings.

## Remarks

If the channel is currently playing, this function returns 1. Otherwise it
returns 0.

If the specified channel is -1, all channels are checked, and this function
returns the number of channels currently playing.

You may not specify MAX_CHANNEL_POST for a channel.

Paused channels are treated as playing, even though they are not currently
making forward progress in mixing.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

