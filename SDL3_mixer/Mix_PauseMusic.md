###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_PauseMusic

Pause the music stream.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
void Mix_PauseMusic(void);
```

## Remarks

Pausing the music stream will prevent further playback of the assigned
music object, but will maintain the object's current mixing position. When
resumed, this channel will continue to mix the music where it left off.

Paused music can be resumed by calling
[Mix_ResumeMusic](Mix_ResumeMusic)().

It is legal to halt paused music. Playing a new music object when music is
paused will replace the current music and unpause the music stream.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

