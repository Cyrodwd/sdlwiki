###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetRectIntersection

Calculate the intersection of two rectangles.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
bool SDL_GetRectIntersection(const SDL_Rect *A, const SDL_Rect *B, SDL_Rect *result);
```

## Function Parameters

|                              |            |                                                                                              |
| ---------------------------- | ---------- | -------------------------------------------------------------------------------------------- |
| const [SDL_Rect](SDL_Rect) * | **A**      | an [SDL_Rect](SDL_Rect) structure representing the first rectangle.                          |
| const [SDL_Rect](SDL_Rect) * | **B**      | an [SDL_Rect](SDL_Rect) structure representing the second rectangle.                         |
| [SDL_Rect](SDL_Rect) *       | **result** | an [SDL_Rect](SDL_Rect) structure filled in with the intersection of rectangles `A` and `B`. |

## Return Value

(bool) Returns true if there is an intersection, false otherwise.

## Remarks

If `result` is NULL then this function will return false.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_HasRectIntersection](SDL_HasRectIntersection)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

