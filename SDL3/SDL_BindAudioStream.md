###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_BindAudioStream

Bind a single audio stream to an audio device.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
bool SDL_BindAudioStream(SDL_AudioDeviceID devid, SDL_AudioStream *stream);
```

## Function Parameters

|                                        |            |                                      |
| -------------------------------------- | ---------- | ------------------------------------ |
| [SDL_AudioDeviceID](SDL_AudioDeviceID) | **devid**  | an audio device to bind a stream to. |
| [SDL_AudioStream](SDL_AudioStream) *   | **stream** | an audio stream to bind to a device. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This is a convenience function, equivalent to calling
`SDL_BindAudioStreams(devid, &stream, 1)`.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_BindAudioStreams](SDL_BindAudioStreams)
- [SDL_UnbindAudioStream](SDL_UnbindAudioStream)
- [SDL_GetAudioStreamDevice](SDL_GetAudioStreamDevice)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

