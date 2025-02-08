# SDL_WriteU8

Use this function to write a byte to an [SDL_RWops](SDL_RWops).

## Header File

Defined in [SDL_rwops.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_rwops.h)

## Syntax

```c
size_t SDL_WriteU8(SDL_RWops * dst, Uint8 value);
```

## Function Parameters

|                          |           |                                         |
| ------------------------ | --------- | --------------------------------------- |
| [SDL_RWops](SDL_RWops) * | **dst**   | the [SDL_RWops](SDL_RWops) to write to. |
| Uint8                    | **value** | the byte value to write.                |

## Return Value

(size_t) Returns 1 on success or 0 on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_ReadU8](SDL_ReadU8)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryRWOPS](CategoryRWOPS)

