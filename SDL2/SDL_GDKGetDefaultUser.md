# SDL_GDKGetDefaultUser

Gets a reference to the default user handle for GDK.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
int SDL_GDKGetDefaultUser(XUserHandle * outUserHandle);
```

## Function Parameters

|               |                   |                                                         |
| ------------- | ----------------- | ------------------------------------------------------- |
| XUserHandle * | **outUserHandle** | a pointer to be filled in with the default user handle. |

## Return Value

(int) Returns 0 if success, -1 if any error occurs.

## Remarks

This is effectively a synchronous version of XUserAddAsync, which always
prefers the default user and allows a sign-in UI.

## Version

This function is available since SDL 2.28.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

