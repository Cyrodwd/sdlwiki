###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_AudioStreamPut

Add data to be converted/resampled to the stream.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
int SDL_AudioStreamPut(SDL_AudioStream *stream, const void *buf, int len);
```

## Function Parameters

|                                      |            |                                              |
| ------------------------------------ | ---------- | -------------------------------------------- |
| [SDL_AudioStream](SDL_AudioStream) * | **stream** | The stream the audio data is being added to. |
| const void *                         | **buf**    | A pointer to the audio data to add.          |
| int                                  | **len**    | The number of bytes to write to the stream.  |

## Return Value

(int) Returns 0 on success, or -1 on error.

## Version

This function is available since SDL 2.0.7.

## See Also

- [SDL_NewAudioStream](SDL_NewAudioStream)
- [SDL_AudioStreamGet](SDL_AudioStreamGet)
- [SDL_AudioStreamAvailable](SDL_AudioStreamAvailable)
- [SDL_AudioStreamFlush](SDL_AudioStreamFlush)
- [SDL_AudioStreamClear](SDL_AudioStreamClear)
- [SDL_FreeAudioStream](SDL_FreeAudioStream)


## (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

