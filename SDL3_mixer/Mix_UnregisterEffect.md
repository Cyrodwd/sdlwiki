###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_UnregisterEffect

Explicitly unregister a special effect function.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_UnregisterEffect(int channel, Mix_EffectFunc_t f);
```

## Function Parameters

|                                      |             |                                                                                  |
| ------------------------------------ | ----------- | -------------------------------------------------------------------------------- |
| int                                  | **channel** | the channel to unregister an effect on, or [MIX_CHANNEL_POST](MIX_CHANNEL_POST). |
| [Mix_EffectFunc_t](Mix_EffectFunc_t) | **f**       | effect the callback stop calling in future mixing iterations.                    |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information.

## Remarks

You may not need to call this at all, unless you need to stop an effect
from processing in the middle of a chunk's playback.

Posteffects are never implicitly unregistered as they are for channels (as
the output stream does not have an end), but they may be explicitly
unregistered through this function by specifying
[MIX_CHANNEL_POST](MIX_CHANNEL_POST) for a channel.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

