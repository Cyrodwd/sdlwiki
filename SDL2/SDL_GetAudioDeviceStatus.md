###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_GetAudioDeviceStatus

Use this function to get the current audio state of an audio device.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
SDL_AudioStatus SDL_GetAudioDeviceStatus(SDL_AudioDeviceID dev);
```

## Function Parameters

|                                        |         |                                                                                                |
| -------------------------------------- | ------- | ---------------------------------------------------------------------------------------------- |
| [SDL_AudioDeviceID](SDL_AudioDeviceID) | **dev** | the ID of an audio device previously opened with [SDL_OpenAudioDevice](SDL_OpenAudioDevice)(). |

## Return Value

([SDL_AudioStatus](SDL_AudioStatus)) Returns the
[SDL_AudioStatus](SDL_AudioStatus) of the specified audio device.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_PauseAudioDevice](SDL_PauseAudioDevice)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

