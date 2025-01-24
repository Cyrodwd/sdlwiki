# SDL_GlobStorageDirectory

Enumerate a directory tree, filtered by pattern, and return a list.

## Header File

Defined in [<SDL3/SDL_storage.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_storage.h)

## Syntax

```c
char ** SDL_GlobStorageDirectory(SDL_Storage *storage, const char *path, const char *pattern, SDL_GlobFlags flags, int *count);
```

## Function Parameters

|                                |             |                                                                                   |
| ------------------------------ | ----------- | --------------------------------------------------------------------------------- |
| [SDL_Storage](SDL_Storage) *   | **storage** | a storage container.                                                              |
| const char *                   | **path**    | the path of the directory to enumerate, or NULL for the root.                     |
| const char *                   | **pattern** | the pattern that files in the directory must match. Can be NULL.                  |
| [SDL_GlobFlags](SDL_GlobFlags) | **flags**   | `SDL_GLOB_*` bitflags that affect this search.                                    |
| int *                          | **count**   | on return, will be set to the number of items in the returned array. Can be NULL. |

## Return Value

(char **) Returns an array of strings on success or NULL on failure; call
[SDL_GetError](SDL_GetError)() for more information. The caller should pass
the returned pointer to [SDL_free](SDL_free) when done with it. This is a
single allocation that should be freed with [SDL_free](SDL_free)() when it
is no longer needed.

## Remarks

Files are filtered out if they don't match the string in `pattern`, which
may contain wildcard characters '*' (match everything) and '?' (match one
character). If pattern is NULL, no filtering is done and all results are
returned. Subdirectories are permitted, and are specified with a path
separator of '/'. Wildcard characters '*' and '?' never match a path
separator.

`flags` may be set to [SDL_GLOB_CASEINSENSITIVE](SDL_GLOB_CASEINSENSITIVE)
to make the pattern matching case-insensitive.

The returned array is always NULL-terminated, for your iterating
convenience, but if `count` is non-NULL, on return it will contain the
number of items in the array, not counting the NULL terminator.

If `path` is NULL, this is treated as a request to enumerate the root of
the storage container's tree. An empty string also works for this.

## Thread Safety

It is safe to call this function from any thread, assuming the `storage`
object is thread-safe.

## Version

This function is available since SDL 3.2.0.

## (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)



----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryStorage](CategoryStorage)

