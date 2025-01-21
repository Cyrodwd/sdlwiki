###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetAudioDriver

Use this function to get the name of a built in audio driver.

## Header File

Defined in [<SDL3/SDL_audio.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_audio.h)

## Syntax

```c
const char * SDL_GetAudioDriver(int index);
```

## Function Parameters

|     |           |                                                                                                                   |
| --- | --------- | ----------------------------------------------------------------------------------------------------------------- |
| int | **index** | the index of the audio driver; the value ranges from 0 to [SDL_GetNumAudioDrivers](SDL_GetNumAudioDrivers)() - 1. |

## Return Value

(const char *) Returns the name of the audio driver at the requested index,
or NULL if an invalid index was specified.

## Remarks

The list of audio drivers is given in the order that they are normally
initialized by default; the drivers that seem more reasonable to choose
first (as far as the SDL developers believe) are earlier in the list.

The names of drivers are all simple, low-ASCII identifiers, like "alsa",
"coreaudio" or "wasapi". These never have Unicode characters, and are not
meant to be proper names.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_GetNumAudioDrivers](SDL_GetNumAudioDrivers)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

