###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_PlayMusic

Play a new music object.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
bool Mix_PlayMusic(Mix_Music *music, int loops);
```

## Function Parameters

|                          |           |                                                                           |
| ------------------------ | --------- | ------------------------------------------------------------------------- |
| [Mix_Music](Mix_Music) * | **music** | the new music object to schedule for mixing.                              |
| int                      | **loops** | the number of loops to play the music for (0 means "play once and stop"). |

## Return Value

(bool) Returns true on success or false on failure; call SDL_GetError() for
more information.

## Remarks

This will schedule the music object to begin mixing for playback.

There is only ever one music object playing at a time; if this is called
when another music object is playing, the currently-playing music is halted
and the new music will replace it.

Please note that if the currently-playing music is in the process of fading
out (via [Mix_FadeOutMusic](Mix_FadeOutMusic)()), this function will
*block* until the fade completes. If you need to avoid this, be sure to
call [Mix_HaltMusic](Mix_HaltMusic)() before starting new music.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

