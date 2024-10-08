###### (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_PauseAudioDevice

Use this function to pause and unpause audio playback on a specified device.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
void SDL_PauseAudioDevice(SDL_AudioDeviceID dev,
                          int pause_on);
```

## Function Parameters

|                                        |              |                                                                  |
| -------------------------------------- | ------------ | ---------------------------------------------------------------- |
| [SDL_AudioDeviceID](SDL_AudioDeviceID) | **dev**      | a device opened by [SDL_OpenAudioDevice](SDL_OpenAudioDevice)(). |
| int                                    | **pause_on** | non-zero to pause, 0 to unpause.                                 |

## Remarks

This function pauses and unpauses the audio callback processing for a given
device. Newly-opened audio devices start in the paused state, so you must
call this function with **pause_on**=0 after opening the specified audio
device to start playing sound. This allows you to safely initialize data
for your callback function after opening the audio device. Silence will be
written to the audio device while paused, and the audio callback is
guaranteed to not be called. Pausing one device does not prevent other
unpaused devices from running their callbacks.

Pausing state does not stack; even if you pause a device several times, a
single unpause will start the device playing again, and vice versa. This is
different from how [SDL_LockAudioDevice](SDL_LockAudioDevice)() works.

If you just need to protect a few variables from race conditions vs your
callback, you shouldn't pause the audio device, as it will lead to dropouts
in the audio playback. Instead, you should use
[SDL_LockAudioDevice](SDL_LockAudioDevice)().

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_LockAudioDevice](SDL_LockAudioDevice)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

