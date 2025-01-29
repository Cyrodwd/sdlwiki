# SDL_ResumeAudioDevice

Use this function to unpause audio playback on a specified device.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
bool SDL_ResumeAudioDevice(SDL_AudioDeviceID devid);
```

## Function Parameters

|                                        |           |                                                                  |
| -------------------------------------- | --------- | ---------------------------------------------------------------- |
| [SDL_AudioDeviceID](SDL_AudioDeviceID) | **devid** | a device opened by [SDL_OpenAudioDevice](SDL_OpenAudioDevice)(). |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This function unpauses audio processing for a given device that has
previously been paused with [SDL_PauseAudioDevice](SDL_PauseAudioDevice)().
Once unpaused, any bound audio streams will begin to progress again, and
audio can be generated.

Unlike in SDL2, audio devices start in an _unpaused_ state, since an app
has to bind a stream before any audio will flow. Unpausing an unpaused
device is a legal no-op.

Physical devices can not be paused or unpaused, only logical devices
created through [SDL_OpenAudioDevice](SDL_OpenAudioDevice)() can be.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_AudioDevicePaused](SDL_AudioDevicePaused)
- [SDL_PauseAudioDevice](SDL_PauseAudioDevice)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

