###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_CreateSystemCursor

Create a system cursor.

## Header File

Defined in [<SDL3/SDL_mouse.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_mouse.h)

## Syntax

```c
SDL_Cursor * SDL_CreateSystemCursor(SDL_SystemCursor id);
```

## Function Parameters

|                                      |        |                                                     |
| ------------------------------------ | ------ | --------------------------------------------------- |
| [SDL_SystemCursor](SDL_SystemCursor) | **id** | an [SDL_SystemCursor](SDL_SystemCursor) enum value. |

## Return Value

([SDL_Cursor](SDL_Cursor) *) Returns a cursor on success or NULL on
failure; call [SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 3.0.0.

## Code Examples

```c
SDL_Cursor* cursor;
cursor = SDL_CreateSystemCursor(SDL_SYSTEM_CURSOR_POINTER);
SDL_SetCursor(cursor);
```

## See Also

- [SDL_DestroyCursor](SDL_DestroyCursor)


## (This is the documentation for SDL3, which is under heavy development and the API is changing! [SDL2](https://wiki.libsdl.org/SDL2/) is the current stable version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryMouse](CategoryMouse)

