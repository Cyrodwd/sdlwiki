# SDL_GetRectAndLineIntersection

Calculate the intersection of a rectangle and line segment.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
bool SDL_GetRectAndLineIntersection(const SDL_Rect *rect, int *X1, int *Y1, int *X2, int *Y2);
```

## Function Parameters

|                              |          |                                                                            |
| ---------------------------- | -------- | -------------------------------------------------------------------------- |
| const [SDL_Rect](SDL_Rect) * | **rect** | an [SDL_Rect](SDL_Rect) structure representing the rectangle to intersect. |
| int *                        | **X1**   | a pointer to the starting X-coordinate of the line.                        |
| int *                        | **Y1**   | a pointer to the starting Y-coordinate of the line.                        |
| int *                        | **X2**   | a pointer to the ending X-coordinate of the line.                          |
| int *                        | **Y2**   | a pointer to the ending Y-coordinate of the line.                          |

## Return Value

(bool) Returns true if there is an intersection, false otherwise.

## Remarks

This function is used to clip a line segment to a rectangle. A line segment
contained entirely within the rectangle or that does not intersect will
remain unchanged. A line segment that crosses the rectangle at either or
both ends will be clipped to the boundary of the rectangle and the new
coordinates saved in `X1`, `Y1`, `X2`, and/or `Y2` as necessary.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

