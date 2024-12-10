###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_FadingChannel

Query the fading status of a channel.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
Mix_Fading Mix_FadingChannel(int which);
```

## Function Parameters

|     |           |                       |
| --- | --------- | --------------------- |
| int | **which** | the channel to query. |

## Return Value

([Mix_Fading](Mix_Fading)) Returns the current fading status of the
channel.

## Remarks

This reports one of three values:

- [`MIX_NO_FADING`](MIX_NO_FADING)
- [`MIX_FADING_OUT`](MIX_FADING_OUT)
- [`MIX_FADING_IN`](MIX_FADING_IN)

If nothing is currently playing on the channel, or an invalid channel is
specified, this returns [`MIX_NO_FADING`](MIX_NO_FADING).

You may not specify MAX_CHANNEL_POST for a channel.

You may not specify -1 for all channels; only individual channels may be
queried.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

