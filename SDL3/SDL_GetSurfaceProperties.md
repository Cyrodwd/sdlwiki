###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetSurfaceProperties

Get the properties associated with a surface.

## Header File

Defined in [<SDL3/SDL_surface.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_surface.h)

## Syntax

```c
SDL_PropertiesID SDL_GetSurfaceProperties(SDL_Surface *surface);
```

## Function Parameters

|                              |             |                                                    |
| ---------------------------- | ----------- | -------------------------------------------------- |
| [SDL_Surface](SDL_Surface) * | **surface** | the [SDL_Surface](SDL_Surface) structure to query. |

## Return Value

([SDL_PropertiesID](SDL_PropertiesID)) Returns a valid property ID on
success or 0 on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

The following properties are understood by SDL:

- [`SDL_PROP_SURFACE_SDR_WHITE_POINT_FLOAT`](SDL_PROP_SURFACE_SDR_WHITE_POINT_FLOAT):
  for HDR10 and floating point surfaces, this defines the value of 100%
  diffuse white, with higher values being displayed in the High Dynamic
  Range headroom. This defaults to 203 for HDR10 surfaces and 1.0 for
  floating point surfaces.
- [`SDL_PROP_SURFACE_HDR_HEADROOM_FLOAT`](SDL_PROP_SURFACE_HDR_HEADROOM_FLOAT):
  for HDR10 and floating point surfaces, this defines the maximum dynamic
  range used by the content, in terms of the SDR white point. This defaults
  to 0.0, which disables tone mapping.
- [`SDL_PROP_SURFACE_TONEMAP_OPERATOR_STRING`](SDL_PROP_SURFACE_TONEMAP_OPERATOR_STRING):
  the tone mapping operator used when compressing from a surface with high
  dynamic range to another with lower dynamic range. Currently this
  supports "chrome", which uses the same tone mapping that Chrome uses for
  HDR content, the form "*=N", where N is a floating point scale factor
  applied in linear space, and "none", which disables tone mapping. This
  defaults to "chrome".

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySurface](CategorySurface)

