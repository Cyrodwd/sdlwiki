# SDL_HitTestResult

Possible return values from the [SDL_HitTest](SDL_HitTest) callback.

## Header File

Defined in [<SDL3/SDL_video.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_video.h)

## Syntax

```c
typedef enum SDL_HitTestResult
{
    SDL_HITTEST_NORMAL,             /**< Region is normal. No special properties. */
    SDL_HITTEST_DRAGGABLE,          /**< Region can drag entire window. */
    SDL_HITTEST_RESIZE_TOPLEFT,     /**< Region is the resizable top-left corner border. */
    SDL_HITTEST_RESIZE_TOP,         /**< Region is the resizable top border. */
    SDL_HITTEST_RESIZE_TOPRIGHT,    /**< Region is the resizable top-right corner border. */
    SDL_HITTEST_RESIZE_RIGHT,       /**< Region is the resizable right border. */
    SDL_HITTEST_RESIZE_BOTTOMRIGHT, /**< Region is the resizable bottom-right corner border. */
    SDL_HITTEST_RESIZE_BOTTOM,      /**< Region is the resizable bottom border. */
    SDL_HITTEST_RESIZE_BOTTOMLEFT,  /**< Region is the resizable bottom-left corner border. */
    SDL_HITTEST_RESIZE_LEFT         /**< Region is the resizable left border. */
} SDL_HitTestResult;
```

## Thread Safety

This function should only be called on the main thread.

## Version

This enum is available since SDL 3.2.0.

## See Also

- [SDL_HitTest](SDL_HitTest)






----
[CategoryAPI](CategoryAPI), [CategoryAPIEnum](CategoryAPIEnum), [CategoryVideo](CategoryVideo)

