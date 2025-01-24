# SDL_OpenStorage

Opens up a container using a client-provided storage interface.

## Header File

Defined in [<SDL3/SDL_storage.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_storage.h)

## Syntax

```c
SDL_Storage * SDL_OpenStorage(const SDL_StorageInterface *iface, void *userdata);
```

## Function Parameters

|                                                      |              |                                                                                                           |
| ---------------------------------------------------- | ------------ | --------------------------------------------------------------------------------------------------------- |
| const [SDL_StorageInterface](SDL_StorageInterface) * | **iface**    | the interface that implements this storage, initialized using [SDL_INIT_INTERFACE](SDL_INIT_INTERFACE)(). |
| void *                                               | **userdata** | the pointer that will be passed to the interface functions.                                               |

## Return Value

([SDL_Storage](SDL_Storage) *) Returns a storage container on success or
NULL on failure; call [SDL_GetError](SDL_GetError)() for more information.

## Remarks

Applications do not need to use this function unless they are providing
their own [SDL_Storage](SDL_Storage) implementation. If you just need an
[SDL_Storage](SDL_Storage), you should use the built-in implementations in
SDL, like [SDL_OpenTitleStorage](SDL_OpenTitleStorage)() or
[SDL_OpenUserStorage](SDL_OpenUserStorage)().

This function makes a copy of `iface` and the caller does not need to keep
it around after this call.

## Version

This function is available since SDL 3.2.0.

## See Also

- [SDL_CloseStorage](SDL_CloseStorage)
- [SDL_GetStorageFileSize](SDL_GetStorageFileSize)
- [SDL_GetStorageSpaceRemaining](SDL_GetStorageSpaceRemaining)
- [SDL_INIT_INTERFACE](SDL_INIT_INTERFACE)
- [SDL_ReadStorageFile](SDL_ReadStorageFile)
- [SDL_StorageReady](SDL_StorageReady)
- [SDL_WriteStorageFile](SDL_WriteStorageFile)


## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStorage](CategoryStorage)

