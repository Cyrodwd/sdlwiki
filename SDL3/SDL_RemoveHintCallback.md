# SDL_RemoveHintCallback

Remove a function watching a particular hint.

## Header File

Defined in [<SDL3/SDL_hints.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hints.h)

## Syntax

```c
void SDL_RemoveHintCallback(const char *name,
                         SDL_HintCallback callback,
                         void *userdata);
```

## Function Parameters

|                                      |              |                                                                                                   |
| ------------------------------------ | ------------ | ------------------------------------------------------------------------------------------------- |
| const char *                         | **name**     | the hint being watched.                                                                           |
| [SDL_HintCallback](SDL_HintCallback) | **callback** | an [SDL_HintCallback](SDL_HintCallback) function that will be called when the hint value changes. |
| void *                               | **userdata** | a pointer being passed to the callback function.                                                  |

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_AddHintCallback](SDL_AddHintCallback)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHints](CategoryHints)

