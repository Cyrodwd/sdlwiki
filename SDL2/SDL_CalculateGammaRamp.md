# SDL_CalculateGammaRamp

Calculate a 256 entry gamma ramp for a gamma value.

## Header File

Defined in [SDL_pixels.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_pixels.h)

## Syntax

```c
void SDL_CalculateGammaRamp(float gamma, Uint16 * ramp);
```

## Function Parameters

|                    |           |                                                       |
| ------------------ | --------- | ----------------------------------------------------- |
| float              | **gamma** | a gamma value where 0.0 is black and 1.0 is identity. |
| [Uint16](Uint16) * | **ramp**  | an array of 256 values filled in with the gamma ramp. |

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_SetWindowGammaRamp](SDL_SetWindowGammaRamp)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryPixels](CategoryPixels)

