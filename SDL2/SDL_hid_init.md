# SDL_hid_init

Initialize the HIDAPI library.

## Header File

Defined in [SDL_hidapi.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_init(void);
```

## Return Value

(int) Returns 0 on success and -1 on error.

## Remarks

This function initializes the HIDAPI library. Calling it is not strictly
necessary, as it will be called automatically by
[SDL_hid_enumerate](SDL_hid_enumerate)() and any of the
[SDL_hid_open_](SDL_hid_open_)*() functions if it is needed. This function
should be called at the beginning of execution however, if there is a
chance of HIDAPI handles being opened by different threads simultaneously.

Each call to this function should have a matching call to
[SDL_hid_exit](SDL_hid_exit)()

## Version

This function is available since SDL 2.0.18.

## See Also

- [SDL_hid_exit](SDL_hid_exit)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

