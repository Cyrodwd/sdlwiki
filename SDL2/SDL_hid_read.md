# SDL_hid_read

Read an Input report from a HID device.

## Header File

Defined in [SDL_hidapi.h](https://github.com/libsdl-org/SDL/blob/SDL2/include/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_read(SDL_hid_device *dev, unsigned char *data, size_t length);
```

## Function Parameters

|                                    |            |                                                                                                                        |
| ---------------------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------- |
| [SDL_hid_device](SDL_hid_device) * | **dev**    | A device handle returned from [SDL_hid_open](SDL_hid_open)().                                                          |
| unsigned char *                    | **data**   | A buffer to put the read data into.                                                                                    |
| size_t                             | **length** | The number of bytes to read. For devices with multiple reports, make sure to read an extra byte for the report number. |

## Return Value

(int) Returns the actual number of bytes read and -1 on error. If no packet
was available to be read and the handle is in non-blocking mode, this
function returns 0.

## Remarks

Input reports are returned to the host through the INTERRUPT IN endpoint.
The first byte will contain the Report number if the device uses numbered
reports.

## Version

This function is available since SDL 2.0.18.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

