# SDL_DXGIGetOutputInfo

Get the DXGI Adapter and Output indices for the specified display index.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
SDL_bool SDL_DXGIGetOutputInfo( int displayIndex, int *adapterIndex, int *outputIndex );
```

## Function Parameters

|       |                  |                                                   |
| ----- | ---------------- | ------------------------------------------------- |
| int   | **displayIndex** | the display index for which to get both indices.  |
| int * | **adapterIndex** | a pointer to be filled in with the adapter index. |
| int * | **outputIndex**  | a pointer to be filled in with the output index.  |

## Return Value

([SDL_bool](SDL_bool)) Returns [SDL_TRUE](SDL_TRUE) on success or
[SDL_FALSE](SDL_FALSE) on failure; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

The DXGI Adapter and Output indices can be passed to `EnumAdapters` and
`EnumOutputs` respectively to get the objects required to create a DX10 or
DX11 device and swap chain.

Before SDL 2.0.4 this function did not return a value. Since SDL 2.0.4 it
returns an [SDL_bool](SDL_bool).

## Version

This function is available since SDL 2.0.2.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

