###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_OpenUserStorage

Opens up a container for a user's unique read/write filesystem.

## Header File

Defined in [<SDL3/SDL_storage.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_storage.h)

## Syntax

```c
SDL_Storage * SDL_OpenUserStorage(const char *org, const char *app, SDL_PropertiesID props);
```

## Function Parameters

|                                      |           |                                                                |
| ------------------------------------ | --------- | -------------------------------------------------------------- |
| const char *                         | **org**   | the name of your organization.                                 |
| const char *                         | **app**   | the name of your application.                                  |
| [SDL_PropertiesID](SDL_PropertiesID) | **props** | a property list that may contain backend-specific information. |

## Return Value

([SDL_Storage](SDL_Storage) *) Returns a user storage container on success
or NULL on failure; call [SDL_GetError](SDL_GetError)() for more
information.

## Remarks

While title storage can generally be kept open throughout runtime, user
storage should only be opened when the client is ready to read/write files.
This allows the backend to properly batch file operations and flush them
when the container has been closed; ensuring safe and optimal save I/O.

## Version

This function is available since SDL 3.1.3.

## See Also

- [SDL_CloseStorage](SDL_CloseStorage)
- [SDL_GetStorageFileSize](SDL_GetStorageFileSize)
- [SDL_GetStorageSpaceRemaining](SDL_GetStorageSpaceRemaining)
- [SDL_OpenTitleStorage](SDL_OpenTitleStorage)
- [SDL_ReadStorageFile](SDL_ReadStorageFile)
- [SDL_StorageReady](SDL_StorageReady)
- [SDL_WriteStorageFile](SDL_WriteStorageFile)

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStorage](CategoryStorage)

