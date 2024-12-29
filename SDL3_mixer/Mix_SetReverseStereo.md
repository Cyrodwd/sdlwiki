###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_SetReverseStereo

Cause a channel to reverse its stereo.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_SetReverseStereo(int channel, int flip);
```

## Function Parameters

|     |             |                                                                        |
| --- | ----------- | ---------------------------------------------------------------------- |
| int | **channel** | The mixer channel to reverse, or [MIX_CHANNEL_POST](MIX_CHANNEL_POST). |
| int | **flip**    | non-zero to reverse stereo, zero to disable this effect.               |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information. Note that an audio device in mono mode is a no-op, but
this call will return successful in that case.

## Remarks

This is handy if the user has his speakers hooked up backwards, or you
would like to have a trippy sound effect.

Calling this function with `flip` set to non-zero reverses the chunks's
usual channels. If `flip` is zero, the effect is unregistered.

This uses the [Mix_RegisterEffect](Mix_RegisterEffect)() API internally,
and thus is probably more CPU intensive than having the user just plug in
his speakers correctly. [Mix_SetReverseStereo](Mix_SetReverseStereo)()
returns without registering the effect function if the audio device is not
configured for stereo output.

If you specify [MIX_CHANNEL_POST](MIX_CHANNEL_POST) for `channel`, then
this effect is used on the final mixed stream before sending it on to the
audio device (a posteffect).

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

