# SDL_hid_get_report_descriptor

Get a report descriptor from a HID device.

## Header File

Defined in [<SDL3/SDL_hidapi.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_get_report_descriptor(SDL_hid_device *dev, unsigned char *buf, size_t buf_size);
```

## Function Parameters

|                                    |              |                                                               |
| ---------------------------------- | ------------ | ------------------------------------------------------------- |
| [SDL_hid_device](SDL_hid_device) * | **dev**      | a device handle returned from [SDL_hid_open](SDL_hid_open)(). |
| unsigned char *                    | **buf**      | the buffer to copy descriptor into.                           |
| size_t                             | **buf_size** | the size of the buffer in bytes.                              |

## Return Value

(int) Returns the number of bytes actually copied or -1 on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

User has to provide a preallocated buffer where descriptor will be copied
to. The recommended size for a preallocated buffer is 4096 bytes.

## Version

This function is available since SDL 3.2.0.





----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

