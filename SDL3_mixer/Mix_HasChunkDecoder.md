###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_HasChunkDecoder

Check if a chunk decoder is available by name.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_HasChunkDecoder(const char *name);
```

## Function Parameters

|              |          |                            |
| ------------ | -------- | -------------------------- |
| const char * | **name** | the decoder name to query. |

## Return Value

(bool) Returns true if a decoder by that name is available, false
otherwise.

## Remarks

This result can change between builds AND runs of the program, if external
libraries that add functionality become available. You must successfully
call [Mix_OpenAudio](Mix_OpenAudio)() before calling this function, as
decoders are activated at device open time.

Decoder names are arbitrary but also obvious, so you have to know what
you're looking for ahead of time, but usually it's the file extension in
capital letters (some example names are "AIFF", "VOC", "WAV").

## Version

This function is available since SDL_mixer 3.0.0.

## See Also

- [Mix_GetNumChunkDecoders](Mix_GetNumChunkDecoders)
- [Mix_GetChunkDecoder](Mix_GetChunkDecoder)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

