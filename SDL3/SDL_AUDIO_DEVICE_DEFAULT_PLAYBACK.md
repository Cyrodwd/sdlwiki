###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_AUDIO_DEVICE_DEFAULT_PLAYBACK

A value used to request a default playback audio device.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
#define SDL_AUDIO_DEVICE_DEFAULT_PLAYBACK ((SDL_AudioDeviceID) 0xFFFFFFFFu)
```

## Remarks

Several functions that require an [SDL_AudioDeviceID](SDL_AudioDeviceID)
will accept this value to signify the app just wants the system to choose a
default device instead of the app providing a specific one.

## Version

This macro is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryAudio](CategoryAudio)

