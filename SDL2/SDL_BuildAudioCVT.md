# SDL_BuildAudioCVT

Initialize an [SDL_AudioCVT](SDL_AudioCVT) structure for conversion.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
int SDL_BuildAudioCVT(SDL_AudioCVT * cvt,
                      SDL_AudioFormat src_format,
                      Uint8 src_channels,
                      int src_rate,
                      SDL_AudioFormat dst_format,
                      Uint8 dst_channels,
                      int dst_rate);
```

## Function Parameters

|                                    |                  |                                                                                                 |
| ---------------------------------- | ---------------- | ----------------------------------------------------------------------------------------------- |
| [SDL_AudioCVT](SDL_AudioCVT) *     | **cvt**          | an [SDL_AudioCVT](SDL_AudioCVT) structure filled in with audio conversion information.          |
| [SDL_AudioFormat](SDL_AudioFormat) | **src_format**   | the source format of the audio data; for more info see [SDL_AudioFormat](SDL_AudioFormat).      |
| Uint8                              | **src_channels** | the number of channels in the source.                                                           |
| int                                | **src_rate**     | the frequency (sample-frames-per-second) of the source.                                         |
| [SDL_AudioFormat](SDL_AudioFormat) | **dst_format**   | the destination format of the audio data; for more info see [SDL_AudioFormat](SDL_AudioFormat). |
| Uint8                              | **dst_channels** | the number of channels in the destination.                                                      |
| int                                | **dst_rate**     | the frequency (sample-frames-per-second) of the destination.                                    |

## Return Value

(int) Returns 1 if the audio filter is prepared, 0 if no conversion is
needed, or a negative error code on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Before an [SDL_AudioCVT](SDL_AudioCVT) structure can be used to convert
audio data it must be initialized with source and destination information.

This function will zero out every field of the
[SDL_AudioCVT](SDL_AudioCVT), so it must be called before the application
fills in the final buffer information.

Once this function has returned successfully, and reported that a
conversion is necessary, the application fills in the rest of the fields in
[SDL_AudioCVT](SDL_AudioCVT), now that it knows how large a buffer it needs
to allocate, and then can call [SDL_ConvertAudio](SDL_ConvertAudio)() to
complete the conversion.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_ConvertAudio](SDL_ConvertAudio)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

