###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_GetRectEnclosingPoints

Calculate a minimal rectangle enclosing a set of points.

## Header File

Defined in [<SDL3/SDL_rect.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_rect.h)

## Syntax

```c
bool SDL_GetRectEnclosingPoints(const SDL_Point *points, int count, const SDL_Rect *clip, SDL_Rect *result);
```

## Function Parameters

|                                |            |                                                                                   |
| ------------------------------ | ---------- | --------------------------------------------------------------------------------- |
| const [SDL_Point](SDL_Point) * | **points** | an array of [SDL_Point](SDL_Point) structures representing points to be enclosed. |
| int                            | **count**  | the number of structures in the `points` array.                                   |
| const [SDL_Rect](SDL_Rect) *   | **clip**   | an [SDL_Rect](SDL_Rect) used for clipping or NULL to enclose all points.          |
| [SDL_Rect](SDL_Rect) *         | **result** | an [SDL_Rect](SDL_Rect) structure filled in with the minimal enclosing rectangle. |

## Return Value

(bool) Returns true if any points were enclosed or false if all the points
were outside of the clipping rectangle.

## Remarks

If `clip` is not NULL then only points inside of the clipping rectangle are
considered.

## Version

This function is available since SDL 3.2.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

