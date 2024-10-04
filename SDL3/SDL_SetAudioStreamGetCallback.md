###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_SetAudioStreamGetCallback

Set a callback that runs when data is requested from an audio stream.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
bool SDL_SetAudioStreamGetCallback(SDL_AudioStream *stream, SDL_AudioStreamCallback callback, void *userdata);
```

## Function Parameters

|                                                    |              |                                                                           |
| -------------------------------------------------- | ------------ | ------------------------------------------------------------------------- |
| [SDL_AudioStream](SDL_AudioStream) *               | **stream**   | the audio stream to set the new callback on.                              |
| [SDL_AudioStreamCallback](SDL_AudioStreamCallback) | **callback** | the new callback function to call when data is requested from the stream. |
| void *                                             | **userdata** | an opaque pointer provided to the callback for its own personal use.      |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information. This only fails if
`stream` is NULL.

## Remarks

This callback is called _before_ data is obtained from the stream, giving
the callback the chance to add more on-demand.

The callback can (optionally) call
[SDL_PutAudioStreamData](SDL_PutAudioStreamData)() to add more audio to the
stream during this call; if needed, the request that triggered this
callback will obtain the new data immediately.

The callback's `approx_request` argument is roughly how many bytes of
_unconverted_ data (in the stream's input format) is needed by the caller,
although this may overestimate a little for safety. This takes into account
how much is already in the stream and only asks for any extra necessary to
resolve the request, which means the callback may be asked for zero bytes,
and a different amount on each call.

The callback is not required to supply exact amounts; it is allowed to
supply too much or too little or none at all. The caller will get what's
available, up to the amount they requested, regardless of this callback's
outcome.

Clearing or flushing an audio stream does not call this callback.

This function obtains the stream's lock, which means any existing callback
(get or put) in progress will finish running before setting the new
callback.

Setting a NULL function turns off the callback.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_SetAudioStreamPutCallback](SDL_SetAudioStreamPutCallback)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

