# SDL_RecordGesture

Begin recording a gesture on a specified touch device or all touch devices.

## Header File

Defined in [SDL_gesture.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_gesture.h)

## Syntax

```c
int SDL_RecordGesture(SDL_TouchID touchId);
```

## Function Parameters

|                            |             |                                                   |
| -------------------------- | ----------- | ------------------------------------------------- |
| [SDL_TouchID](SDL_TouchID) | **touchId** | the touch device id, or -1 for all touch devices. |

## Return Value

(int) Returns 1 on success or 0 if the specified device could not be found.

## Remarks

If the parameter `touchId` is -1 (i.e., all devices), this function will
always return 1, regardless of whether there actually are any devices.

## Version

This function is available since SDL 2.0.0.

## See Also

- [SDL_GetTouchDevice](SDL_GetTouchDevice)






----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryGesture](CategoryGesture)

