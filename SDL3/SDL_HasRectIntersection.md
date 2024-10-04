###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_HasRectIntersection

Determine whether two rectangles intersect.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
bool SDL_HasRectIntersection(const SDL_Rect *A, const SDL_Rect *B);
```

## Function Parameters

|                              |       |                                                                      |
| ---------------------------- | ----- | -------------------------------------------------------------------- |
| const [SDL_Rect](SDL_Rect) * | **A** | an [SDL_Rect](SDL_Rect) structure representing the first rectangle.  |
| const [SDL_Rect](SDL_Rect) * | **B** | an [SDL_Rect](SDL_Rect) structure representing the second rectangle. |

## Return Value

(bool) Returns true if there is an intersection, false otherwise.

## Remarks

If either pointer is NULL the function will return false.

## Thread Safety

It is safe to call this function from any thread.

## Version

This function is available since SDL 3.0.0.

## See Also

- [SDL_GetRectIntersection](SDL_GetRectIntersection)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

