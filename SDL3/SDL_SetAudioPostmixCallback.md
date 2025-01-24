# SDL_SetAudioPostmixCallback

Set a callback that fires when data is about to be fed to an audio device.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
bool SDL_SetAudioPostmixCallback(SDL_AudioDeviceID devid, SDL_AudioPostmixCallback callback, void *userdata);
```

## Function Parameters

|                                                      |              |                                                         |
| ---------------------------------------------------- | ------------ | ------------------------------------------------------- |
| [SDL_AudioDeviceID](SDL_AudioDeviceID)               | **devid**    | the ID of an opened audio device.                       |
| [SDL_AudioPostmixCallback](SDL_AudioPostmixCallback) | **callback** | a callback function to be called. Can be NULL.          |
| void *                                               | **userdata** | app-controlled pointer passed to callback. Can be NULL. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This is useful for accessing the final mix, perhaps for writing a
visualizer or applying a final effect to the audio data before playback.

The buffer is the final mix of all bound audio streams on an opened device;
this callback will fire regularly for any device that is both opened and
unpaused. If there is no new data to mix, either because no streams are
bound to the device or all the streams are empty, this callback will still
fire with the entire buffer set to silence.

This callback is allowed to make changes to the data; the contents of the
buffer after this call is what is ultimately passed along to the hardware.

The callback is always provided the data in float format (values from -1.0f
to 1.0f), but the number of channels or sample rate may be different than
the format the app requested when opening the device; SDL might have had to
manage a conversion behind the scenes, or the playback might have jumped to
new physical hardware when a system default changed, etc. These details may
change between calls. Accordingly, the size of the buffer might change
between calls as well.

This callback can run at any time, and from any thread; if you need to
serialize access to your app's data, you should provide and use a mutex or
other synchronization device.

All of this to say: there are specific needs this callback can fulfill, but
it is not the simplest interface. Apps should generally provide audio in
their preferred format through an [SDL_AudioStream](SDL_AudioStream) and
let SDL handle the difference.

This function is extremely time-sensitive; the callback should do the least
amount of work possible and return as quickly as it can. The longer the
callback runs, the higher the risk of audio dropouts or other problems.

This function will block until the audio device is in between iterations,
so any existing callback that might be running will finish before this
function sets the new callback and returns.

Setting a NULL callback function disables any previously-set callback.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

