# SDL_UnlockAudio

This function is a legacy means of unlocking the audio device.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
void SDL_UnlockAudio(void);
```

## Remarks

New programs might want to use
[SDL_UnlockAudioDevice](SDL_UnlockAudioDevice)() instead. This function is
equivalent to calling...

```c
SDL_UnlockAudioDevice(1);
```

...and is only useful if you used the legacy
[SDL_OpenAudio](SDL_OpenAudio)() function.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_LockAudio](SDL_LockAudio)
- [SDL_UnlockAudioDevice](SDL_UnlockAudioDevice)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

