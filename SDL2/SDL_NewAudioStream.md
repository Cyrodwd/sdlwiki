# SDL_NewAudioStream

Create a new audio stream.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
SDL_AudioStream * SDL_NewAudioStream(const SDL_AudioFormat src_format,
                   const Uint8 src_channels,
                   const int src_rate,
                   const SDL_AudioFormat dst_format,
                   const Uint8 dst_channels,
                   const int dst_rate);
```

## Function Parameters

|                                          |                  |                                                     |
| ---------------------------------------- | ---------------- | --------------------------------------------------- |
| const [SDL_AudioFormat](SDL_AudioFormat) | **src_format**   | The format of the source audio.                     |
| const Uint8                              | **src_channels** | The number of channels of the source audio.         |
| const int                                | **src_rate**     | The sampling rate of the source audio.              |
| const [SDL_AudioFormat](SDL_AudioFormat) | **dst_format**   | The format of the desired audio output.             |
| const Uint8                              | **dst_channels** | The number of channels of the desired audio output. |
| const int                                | **dst_rate**     | The sampling rate of the desired audio output.      |

## Return Value

([SDL_AudioStream](SDL_AudioStream) *) Returns 0 on success, or -1 on
error.

## Version

This function is available since SDL 2.0.7.

## See Also

- [SDL_AudioStreamPut](SDL_AudioStreamPut)
- [SDL_AudioStreamGet](SDL_AudioStreamGet)
- [SDL_AudioStreamAvailable](SDL_AudioStreamAvailable)
- [SDL_AudioStreamFlush](SDL_AudioStreamFlush)
- [SDL_AudioStreamClear](SDL_AudioStreamClear)
- [SDL_FreeAudioStream](SDL_FreeAudioStream)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

