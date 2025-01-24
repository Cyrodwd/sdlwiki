# SDL_UnionFRect

Calculate the union of two rectangles with float precision.

## Header File

Defined in [SDL_rect.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rect.h)

## Syntax

```c
void SDL_UnionFRect(const SDL_FRect * A,
                    const SDL_FRect * B,
                    SDL_FRect * result);
```

## Function Parameters

|                                |            |                                                                                         |
| ------------------------------ | ---------- | --------------------------------------------------------------------------------------- |
| const [SDL_FRect](SDL_FRect) * | **A**      | an [SDL_FRect](SDL_FRect) structure representing the first rectangle.                   |
| const [SDL_FRect](SDL_FRect) * | **B**      | an [SDL_FRect](SDL_FRect) structure representing the second rectangle.                  |
| [SDL_FRect](SDL_FRect) *       | **result** | an [SDL_FRect](SDL_FRect) structure filled in with the union of rectangles `A` and `B`. |

## Version

This function is available since SDL 2.0.22.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRect](CategoryRect)

