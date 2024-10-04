###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
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


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

