# SDL_GetAudioDeviceSpec

Get the preferred audio format of a specific audio device.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
int SDL_GetAudioDeviceSpec(int index,
                           int iscapture,
                           SDL_AudioSpec *spec);
```

## Function Parameters

|                                  |               |                                                                                                                     |
| -------------------------------- | ------------- | ------------------------------------------------------------------------------------------------------------------- |
| int                              | **index**     | the index of the audio device; valid values range from 0 to [SDL_GetNumAudioDevices](SDL_GetNumAudioDevices)() - 1. |
| int                              | **iscapture** | non-zero to query the list of recording devices, zero to query the list of output devices.                          |
| [SDL_AudioSpec](SDL_AudioSpec) * | **spec**      | The [SDL_AudioSpec](SDL_AudioSpec) to be initialized by this function.                                              |

## Return Value

(int) Returns 0 on success, nonzero on error.

## Remarks

This function is only valid after a successfully initializing the audio
subsystem. The values returned by this function reflect the latest call to
[SDL_GetNumAudioDevices](SDL_GetNumAudioDevices)(); re-call that function
to redetect available hardware.

`spec` will be filled with the sample rate, sample format, and channel
count.

## Version

This function is available since SDL 2.0.16.

## See Also

- [SDL_GetNumAudioDevices](SDL_GetNumAudioDevices)
- [SDL_GetDefaultAudioInfo](SDL_GetDefaultAudioInfo)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

