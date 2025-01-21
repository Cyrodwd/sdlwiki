###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_OpenTitleStorage

Opens up a read-only container for the application's filesystem.

## Header File

Defined in [<SDL3/SDL_storage.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_storage.h)

## Syntax

```c
SDL_Storage * SDL_OpenTitleStorage(const char *override, SDL_PropertiesID props);
```

## Function Parameters

|                                      |              |                                                                |
| ------------------------------------ | ------------ | -------------------------------------------------------------- |
| const char *                         | **override** | a path to override the backend's default title root.           |
| [SDL_PropertiesID](SDL_PropertiesID) | **props**    | a property list that may contain backend-specific information. |

## Return Value

([SDL_Storage](SDL_Storage) *) Returns a title storage container on success
or NULL on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_CloseStorage](SDL_CloseStorage)
- [SDL_GetStorageFileSize](SDL_GetStorageFileSize)
- [SDL_OpenUserStorage](SDL_OpenUserStorage)
- [SDL_ReadStorageFile](SDL_ReadStorageFile)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStorage](CategoryStorage)

