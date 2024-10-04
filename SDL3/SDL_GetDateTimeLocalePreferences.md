###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetDateTimeLocalePreferences

Gets the current preferred date and time format for the system locale.

## Header File

Defined in [<SDL3/SDL_time.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_time.h)

## Syntax

```c
bool SDL_GetDateTimeLocalePreferences(SDL_DateFormat *dateFormat, SDL_TimeFormat *timeFormat);
```

## Function Parameters

|                                    |                |                                                                                                  |
| ---------------------------------- | -------------- | ------------------------------------------------------------------------------------------------ |
| [SDL_DateFormat](SDL_DateFormat) * | **dateFormat** | a pointer to the [SDL_DateFormat](SDL_DateFormat) to hold the returned date format, may be NULL. |
| [SDL_TimeFormat](SDL_TimeFormat) * | **timeFormat** | a pointer to the [SDL_TimeFormat](SDL_TimeFormat) to hold the returned time format, may be NULL. |

## Return Value

(bool) Returns true on success or false on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

This might be a "slow" call that has to query the operating system. It's
best to ask for this once and save the results. However, the preferred
formats can change, usually because the user has changed a system
preference outside of your program.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryTime](CategoryTime)

