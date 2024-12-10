###### (This function is part of SDL_mixer, a separate library from SDL.)
# Mix_ExpireChannel

Change the expiration delay for a particular channel.

## Header File

Defined in [<SDL3_mixer/SDL_mixer.h>](https://github.com/libsdl-org/SDL_mixer/blob/main/include/SDL3_mixer/SDL_mixer.h)

## Syntax

```c
int Mix_ExpireChannel(int channel, int ticks);
```

## Function Parameters

|     |             |                                                                                     |
| --- | ----------- | ----------------------------------------------------------------------------------- |
| int | **channel** | the channel to change the expiration time on.                                       |
| int | **ticks**   | number of milliseconds from now to let channel play before halting, -1 to not halt. |

## Return Value

(int) Returns the number of channels that changed expirations.

## Remarks

The channel will halt after the 'ticks' milliseconds have elapsed, or
remove the expiration if 'ticks' is -1.

This overrides the value passed to the fourth parameter of
[Mix_PlayChannelTimed](Mix_PlayChannelTimed)().

Specifying a channel of -1 will set an expiration for _all_ channels.

Any halted channels will have any currently-registered effects
deregistered, and will call any callback specified by
[Mix_ChannelFinished](Mix_ChannelFinished)() once the halt occurs.

Note that this function does not block for the number of ticks requested;
it just schedules the chunk to expire and notes the time for the mixer to
manage later, and returns immediately.

## Version

This function is available since SDL_mixer 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySDLMixer](CategorySDLMixer)

