###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_ConvertAudioSamples

Convert some audio data of one format to another format.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
bool SDL_ConvertAudioSamples(const SDL_AudioSpec *src_spec, const Uint8 *src_data, int src_len, const SDL_AudioSpec *dst_spec, Uint8 **dst_data, int *dst_len);
```

## Function Parameters

|                                        |              |                                                                                                                                      |
| -------------------------------------- | ------------ | ------------------------------------------------------------------------------------------------------------------------------------ |
| const [SDL_AudioSpec](SDL_AudioSpec) * | **src_spec** | the format details of the input audio.                                                                                               |
| const Uint8 *                          | **src_data** | the audio data to be converted.                                                                                                      |
| int                                    | **src_len**  | the len of src_data.                                                                                                                 |
| const [SDL_AudioSpec](SDL_AudioSpec) * | **dst_spec** | the format details of the output audio.                                                                                              |
| Uint8 **                               | **dst_data** | will be filled with a pointer to converted audio data, which should be freed with [SDL_free](SDL_free)(). On error, it will be NULL. |
| int *                                  | **dst_len**  | will be filled with the len of dst_data.                                                                                             |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Please note that this function is for convenience, but should not be used
to resample audio in blocks, as it will introduce audio artifacts on the
boundaries. You should only use this function if you are converting audio
data in its entirety in one call. If you want to convert audio in smaller
chunks, use an [SDL_AudioStream](SDL_AudioStream), which is designed for
this situation.

Internally, this function creates and destroys an
[SDL_AudioStream](SDL_AudioStream) on each use, so it's also less efficient
than using one directly, if you need to convert multiple times.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

