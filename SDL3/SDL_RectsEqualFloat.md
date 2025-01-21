###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_RectsEqualFloat

Determine whether two floating point rectangles are equal, within a default epsilon.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
SDL_FORCE_INLINE bool SDL_RectsEqualFloat(const SDL_FRect *a, const SDL_FRect *b);
```

## Function Parameters

|                                |       |                               |
| ------------------------------ | ----- | ----------------------------- |
| const [SDL_FRect](SDL_FRect) * | **a** | the first rectangle to test.  |
| const [SDL_FRect](SDL_FRect) * | **b** | the second rectangle to test. |

## Return Value

(bool) Returns true if the rectangles are equal, false otherwise.

## Remarks

Rectangles are considered equal if both are not NULL and each of their x,
y, width and height are within [SDL_FLT_EPSILON](SDL_FLT_EPSILON) of each
other. This is often a reasonable way to compare two floating point
rectangles and deal with the slight precision variations in floating point
calculations that tend to pop up.

Note that this is a forced-inline function in a header, and not a public
API function available in the SDL library (which is to say, the code is
embedded in the calling program and the linker and dynamic loader will not
be able to find this function inside SDL itself).

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_RectsEqualEpsilon](SDL_RectsEqualEpsilon)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

