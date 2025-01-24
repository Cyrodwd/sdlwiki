# SDL_GetAudioStreamQueued

Get the number of bytes currently queued.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
int SDL_GetAudioStreamQueued(SDL_AudioStream *stream);
```

## Function Parameters

|                                      |            |                            |
| ------------------------------------ | ---------- | -------------------------- |
| [SDL_AudioStream](SDL_AudioStream) * | **stream** | the audio stream to query. |

## Return Value

(int) Returns the number of bytes queued or -1 on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This is the number of bytes put into a stream as input, not the number that
can be retrieved as output. Because of several details, it's not possible
to calculate one number directly from the other. If you need to know how
much usable data can be retrieved right now, you should use
[SDL_GetAudioStreamAvailable](SDL_GetAudioStreamAvailable)() and not this
function.

Note that audio streams can change their input format at any time, even if
there is still data queued in a different format, so the returned byte
count will not necessarily match the number of _sample frames_ available.
Users of this API should be aware of format changes they make when feeding
a stream and plan accordingly.

Queued data is not converted until it is consumed by
[SDL_GetAudioStreamData](SDL_GetAudioStreamData), so this value should be
representative of the exact data that was put into the stream.

If the stream has so much data that it would overflow an int, the return
value is clamped to a maximum value, but no queued data is lost; if there
are gigabytes of data queued, the app might need to read some of it with
[SDL_GetAudioStreamData](SDL_GetAudioStreamData) before this function's
return value is no longer clamped.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_PutAudioStreamData](SDL_PutAudioStreamData)
- [SDL_ClearAudioStream](SDL_ClearAudioStream)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

