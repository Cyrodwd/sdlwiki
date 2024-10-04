###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_PointInRectFloat

Determine whether a point resides inside a floating point rectangle.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
SDL_FORCE_INLINE bool SDL_PointInRectFloat(const SDL_FPoint *p, const SDL_FRect *r);
```

## Function Parameters

|                                  |       |                        |
| -------------------------------- | ----- | ---------------------- |
| const [SDL_FPoint](SDL_FPoint) * | **p** | the point to test.     |
| const [SDL_FRect](SDL_FRect) *   | **r** | the rectangle to test. |

## Return Value

(bool) Returns true if `p` is contained by `r`, false otherwise.

## Remarks

A point is considered part of a rectangle if both `p` and `r` are not NULL,
and `p`'s x and y coordinates are >= to the rectangle's top left corner,
and <= the rectangle's x+w and y+h. So a 1x1 rectangle considers point
(0,0) and (0,1) as "inside" and (0,2) as not.

Note that this is a forced-inline function in a header, and not a public
API function available in the SDL library (which is to say, the code is
embedded in the calling program and the linker and dynamic loader will not
be able to find this function inside SDL itself).

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

