###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetAudioDeviceName

Get the human-readable name of a specific audio device.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
const char* SDL_GetAudioDeviceName(int index,
                                   int iscapture);
```

## Function Parameters

|     |               |                                                                                                                     |
| --- | ------------- | ------------------------------------------------------------------------------------------------------------------- |
| int | **index**     | the index of the audio device; valid values range from 0 to [SDL_GetNumAudioDevices](SDL_GetNumAudioDevices)() - 1. |
| int | **iscapture** | non-zero to query the list of recording devices, zero to query the list of output devices.                          |

## Return Value

(const char *) Returns the name of the audio device at the requested index,
or NULL on error.

## Remarks

This function is only valid after successfully initializing the audio
subsystem. The values returned by this function reflect the latest call to
[SDL_GetNumAudioDevices](SDL_GetNumAudioDevices)(); re-call that function
to redetect available hardware.

The string returned by this function is UTF-8 encoded, read-only, and
managed internally. You are not to free it. If you need to keep the string
for any length of time, you should make your own copy of it, as it will be
invalid next time any of several other SDL functions are called.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetNumAudioDevices](SDL_GetNumAudioDevices)
- [SDL_GetDefaultAudioInfo](SDL_GetDefaultAudioInfo)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

