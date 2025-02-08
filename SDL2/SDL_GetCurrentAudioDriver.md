# SDL_GetCurrentAudioDriver

Get the name of the current audio driver.

## Header File

Defined in [SDL_audio.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_audio.h)

## Syntax

```c
const char* SDL_GetCurrentAudioDriver(void);
```

## Return Value

(const char *) Returns the name of the current audio driver or NULL if no
driver has been initialized.

## Remarks

The returned string points to internal static memory and thus never becomes
invalid, even if you quit the audio subsystem and initialize a new driver
(although such a case would return a different static string from another
call to this function, of course). As such, you should not modify or free
the returned string.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_AudioInit](SDL_AudioInit)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryAudio](CategoryAudio)

