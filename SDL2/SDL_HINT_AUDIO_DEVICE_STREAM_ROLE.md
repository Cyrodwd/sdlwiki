# SDL_HINT_AUDIO_DEVICE_STREAM_ROLE

Specify an application role for an audio device.

## Header File

Defined in [SDL_hints.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hints.h)

## Syntax

```c
#define SDL_HINT_AUDIO_DEVICE_STREAM_ROLE "SDL_AUDIO_DEVICE_STREAM_ROLE"
```

## Remarks

Some audio backends (such as Pipewire) allow you to describe the role of
your audio stream. Among other things, this description might show up in a
system control panel or software for displaying and manipulating media
playback/capture graphs.

This hints lets you transmit that information to the OS. The contents of
this hint are used while opening an audio device. You should use a string
that describes your what your program is playing (Game, Music, Movie,
etc...).

Setting this to "" or leaving it unset will have SDL use a reasonable
default: "Game" or something similar.

On targets where this is not supported, this hint does nothing.

## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIMacro](CategoryAPIMacro), [CategoryHints](CategoryHints)

