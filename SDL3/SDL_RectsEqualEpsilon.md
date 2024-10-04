###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_RectsEqualEpsilon

Determine whether two floating point rectangles are equal, within some given epsilon.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
SDL_FORCE_INLINE bool SDL_RectsEqualEpsilon(const SDL_FRect *a, const SDL_FRect *b, const float epsilon);
```

## Function Parameters

|                                |             |                                   |
| ------------------------------ | ----------- | --------------------------------- |
| const [SDL_FRect](SDL_FRect) * | **a**       | the first rectangle to test.      |
| const [SDL_FRect](SDL_FRect) * | **b**       | the second rectangle to test.     |
| const float                    | **epsilon** | the epsilon value for comparison. |

## Return Value

(bool) Returns true if the rectangles are equal, false otherwise.

## Remarks

Rectangles are considered equal if both are not NULL and each of their x,
y, width and height are within `epsilon` of each other. If you don't know
what value to use for `epsilon`, you should call the
[SDL_RectsEqualFloat](SDL_RectsEqualFloat) function instead.

Note that this is a forced-inline function in a header, and not a public
API function available in the SDL library (which is to say, the code is
embedded in the calling program and the linker and dynamic loader will not
be able to find this function inside SDL itself).

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_RectsEqualFloat](SDL_RectsEqualFloat)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

