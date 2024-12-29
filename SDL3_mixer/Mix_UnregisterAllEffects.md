###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_UnregisterAllEffects

Explicitly unregister all special effect functions.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_UnregisterAllEffects(int channel);
```

## Function Parameters

|     |             |                                                                                    |
| --- | ----------- | ---------------------------------------------------------------------------------- |
| int | **channel** | the channel to unregister all effects on, or [MIX_CHANNEL_POST](MIX_CHANNEL_POST). |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information.

## Remarks

You may not need to call this at all, unless you need to stop all effects
from processing in the middle of a chunk's playback.

Note that this will also shut off some internal effect processing, since
[Mix_SetPanning](Mix_SetPanning)() and others may use this API under the
hood. This is called internally when a channel completes playback.
Posteffects are never implicitly unregistered as they are for channels, but
they may be explicitly unregistered through this function by specifying
[MIX_CHANNEL_POST](MIX_CHANNEL_POST) for a channel.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

