###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_DisplayMode

The structure that defines a display mode

## Header File

Defined in [SDL_video.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_video.h)

## Syntax

```c
typedef struct SDL_DisplayMode
{
    Uint32 format;              /**< pixel format */
    int w;                      /**< width, in screen coordinates */
    int h;                      /**< height, in screen coordinates */
    int refresh_rate;           /**< refresh rate (or zero for unspecified) */
    void *driverdata;           /**< driver-specific data, initialize to 0 */
} SDL_DisplayMode;
```

## Code Examples

```c
static int display_in_use = 0; /* Only using first display */

int i, display_mode_count;
SDL_DisplayMode mode;
Uint32 f;

SDL_Log("SDL_GetNumVideoDisplays(): %i", SDL_GetNumVideoDisplays());

display_mode_count = SDL_GetNumDisplayModes(display_in_use);
if (display_mode_count < 1) {
    SDL_Log("SDL_GetNumDisplayModes failed: %s", SDL_GetError());
    return 1;
}
SDL_Log("SDL_GetNumDisplayModes: %i", display_mode_count);

for (i = 0; i < display_mode_count; ++i) {
    if (SDL_GetDisplayMode(display_in_use, i, &mode) != 0) {
        SDL_Log("SDL_GetDisplayMode failed: %s", SDL_GetError());
        return 1;
    }
    f = mode.format;

    SDL_Log("Mode %i\tbpp %i\t%s\t%i x %i",
            i, SDL_BITSPERPIXEL(f),
            SDL_GetPixelFormatName(f),
            mode.w, mode.h);
}
```

## See Also

- [SDL_GetNumDisplayModes](SDL_GetNumDisplayModes)
- [SDL_GetDisplayMode](SDL_GetDisplayMode)
- [SDL_GetDesktopDisplayMode](SDL_GetDesktopDisplayMode)
- [SDL_GetCurrentDisplayMode](SDL_GetCurrentDisplayMode)
- [SDL_GetClosestDisplayMode](SDL_GetClosestDisplayMode)
- [SDL_SetWindowDisplayMode](SDL_SetWindowDisplayMode)
- [SDL_GetWindowDisplayMode](SDL_GetWindowDisplayMode)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIStruct](CategoryAPIStruct), [CategoryVideo](CategoryVideo)

