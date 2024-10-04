###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_LoadWAV

Loads a WAV from a file.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
#define SDL_LoadWAV(file, spec, audio_buf, audio_len) \
    SDL_LoadWAV_RW(SDL_RWFromFile(file, "rb"),1, spec,audio_buf,audio_len)
```

## Remarks

Compatibility convenience function.

## Code Examples

```c++
SDL_AudioSpec wav_spec;
Uint32 wav_length;
Uint8 *wav_buffer;

/* Load the WAV */
if (SDL_LoadWAV("test.wav", &wav_spec, &wav_buffer, &wav_length) == NULL) {
    fprintf(stderr, "Could not open test.wav: %s\n", SDL_GetError());
} else {
    /* Do stuff with the WAV data, and then... */
    SDL_FreeWAV(wav_buffer);
}
```

## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryAudio](CategoryAudio), CategoryAudio


