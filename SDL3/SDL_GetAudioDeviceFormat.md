###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetAudioDeviceFormat

Get the current audio format of a specific audio device.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
bool SDL_GetAudioDeviceFormat(SDL_AudioDeviceID devid, SDL_AudioSpec *spec, int *sample_frames);
```

## Function Parameters

|                                        |                   |                                                                     |
| -------------------------------------- | ----------------- | ------------------------------------------------------------------- |
| [SDL_AudioDeviceID](SDL_AudioDeviceID) | **devid**         | the instance ID of the device to query.                             |
| [SDL_AudioSpec](SDL_AudioSpec) *       | **spec**          | on return, will be filled with device details.                      |
| int *                                  | **sample_frames** | pointer to store device buffer size, in sample frames. Can be NULL. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

For an opened device, this will report the format the device is currently
using. If the device isn't yet opened, this will report the device's
preferred format (or a reasonable default if this can't be determined).

You may also specify
[SDL_AUDIO_DEVICE_DEFAULT_PLAYBACK](SDL_AUDIO_DEVICE_DEFAULT_PLAYBACK) or
[SDL_AUDIO_DEVICE_DEFAULT_RECORDING](SDL_AUDIO_DEVICE_DEFAULT_RECORDING)
here, which is useful for getting a reasonable recommendation before
opening the system-recommended default device.

You can also use this to request the current device buffer size. This is
specified in sample frames and represents the amount of data SDL will feed
to the physical hardware in each chunk. This can be converted to
milliseconds of audio with the following equation:

`ms = (int) ((((Sint64) frames) * 1000) / spec.freq);`

Buffer size is only important if you need low-level control over the audio
playback timing. Most apps do not need this.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

