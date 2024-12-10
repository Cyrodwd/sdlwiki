###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_GroupAvailable

Finds the first available channel in a group of channels.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
int Mix_GroupAvailable(int tag);
```

## Function Parameters

|     |         |                                                          |
| --- | ------- | -------------------------------------------------------- |
| int | **tag** | an arbitrary value, assigned to channels, to search for. |

## Return Value

(int) Returns first available channel, or -1 if none are available.

## Remarks

A tag is an arbitrary number that can be assigned to several mixer
channels, to form groups of channels.

This function searches all channels with a specified tag, and returns the
channel number of the first one it finds that is currently unused.

If no channels with the specified tag are unused, this function returns -1.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

