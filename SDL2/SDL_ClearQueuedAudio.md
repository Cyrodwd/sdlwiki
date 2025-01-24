# SDL_ClearQueuedAudio

Drop any queued audio data waiting to be sent to the hardware.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
void SDL_ClearQueuedAudio(SDL_AudioDeviceID dev);
```

## Function Parameters

|                                        |         |                                                  |
| -------------------------------------- | ------- | ------------------------------------------------ |
| [SDL_AudioDeviceID](SDL_AudioDeviceID) | **dev** | the device ID of which to clear the audio queue. |

## Remarks

Immediately after this call,
[SDL_GetQueuedAudioSize](SDL_GetQueuedAudioSize)() will return 0. For
output devices, the hardware will start playing silence if more audio isn't
queued. For capture devices, the hardware will start filling the empty
queue with new data if the capture device isn't paused.

This will not prevent playback of queued audio that's already been sent to
the hardware, as we can not undo that, so expect there to be some fraction
of a second of audio that might still be heard. This can be useful if you
want to, say, drop any pending music or any unprocessed microphone input
during a level change in your game.

You may not queue or dequeue audio on a device that is using an
application-supplied callback; calling this function on such a device
always returns 0. You have to use the audio callback or queue audio, but
not both.

You should not call [SDL_LockAudio](SDL_LockAudio)() on the device before
clearing the queue; SDL handles locking internally for this function.

This function always succeeds and thus returns void.

## Version

This function is available since SDL 2.0.4.

## See Also

- [SDL_GetQueuedAudioSize](SDL_GetQueuedAudioSize)
- [SDL_QueueAudio](SDL_QueueAudio)
- [SDL_DequeueAudio](SDL_DequeueAudio)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

