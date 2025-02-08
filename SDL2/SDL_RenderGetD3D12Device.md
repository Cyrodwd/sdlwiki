# SDL_RenderGetD3D12Device

Get the D3D12 device associated with a renderer.

## Header File

Defined in [SDL_system.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_system.h)

## Syntax

```c
ID3D12Device* SDL_RenderGetD3D12Device(SDL_Renderer* renderer);
```

## Function Parameters

|                                |              |                                                             |
| ------------------------------ | ------------ | ----------------------------------------------------------- |
| [SDL_Renderer](SDL_Renderer) * | **renderer** | the renderer from which to get the associated D3D12 device. |

## Return Value

(ID3D12Device *) Returns the D3D12 device associated with given renderer or
NULL if it is not a D3D12 renderer; call [SDL_GetError](SDL_GetError)() for
more information.

## Remarks

Once you are done using the device, you should release it to avoid a
resource leak.

## Version

This function is available since SDL 2.24.0.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategorySystem](CategorySystem)

