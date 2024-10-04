###### (This is the legacy documentation for stable SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)
# SDL_CalculateGammaRamp

Calculate a 256 entry gamma ramp for a gamma value.

## Header File

Defined in [SDL_pixels.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_pixels.h)

## Syntax

```c
void SDL_CalculateGammaRamp(float gamma, Uint16 * ramp);
```

## Function Parameters

|          |           |                                                       |
| -------- | --------- | ----------------------------------------------------- |
| float    | **gamma** | a gamma value where 0.0 is black and 1.0 is identity. |
| Uint16 * | **ramp**  | an array of 256 values filled in with the gamma ramp. |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetWindowGammaRamp](SDL_SetWindowGammaRamp)


## (This is the legacy documentation for stable SDL2, the current stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current development version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

