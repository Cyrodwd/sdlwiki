# SDL_HasIntersection

Determine whether two rectangles intersect.

## Header File

Defined in [SDL_rect.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rect.h)

## Syntax

```c
SDL_bool SDL_HasIntersection(const SDL_Rect * A,
                             const SDL_Rect * B);
```

## Function Parameters

|                              |       |                                                                      |
| ---------------------------- | ----- | -------------------------------------------------------------------- |
| const [SDL_Rect](SDL_Rect) * | **A** | an [SDL_Rect](SDL_Rect) structure representing the first rectangle.  |
| const [SDL_Rect](SDL_Rect) * | **B** | an [SDL_Rect](SDL_Rect) structure representing the second rectangle. |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) if there is an
intersection, [SDL_FALSE](SDL_FALSE) otherwise.

## Remarks

If either pointer is NULL the function will return [SDL_FALSE](SDL_FALSE).

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_IntersectRect](SDL_IntersectRect)


## (This is the legacy documentation for SDL2, the previous stable version; [SDL3](https://wiki.libsdl.org/SDL3/) is the current stable version.)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

