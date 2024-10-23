###### (This is the documentation for SDL3, which is the current stable version. [SDL2](https://wiki.libsdl.org/SDL2/) was the previous version!)
# SDL_hid_get_feature_report

Get a feature report from a HID device.

## Header File

Defined in [<SDL3/SDL_hidapi.h>](https://github.com/libsdl-org/SDL/blob/main/include/SDL3/SDL_hidapi.h)

## Syntax

```c
int SDL_hid_get_feature_report(SDL_hid_device *dev, unsigned char *data, size_t length);
```

## Function Parameters

|                                    |            |                                                                                                                                                                                                      |
| ---------------------------------- | ---------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| [SDL_hid_device](SDL_hid_device) * | **dev**    | a device handle returned from [SDL_hid_open](SDL_hid_open)().                                                                                                                                        |
| unsigned char *                    | **data**   | a buffer to put the read data into, including the Report ID. Set the first byte of `data` to the Report ID of the report to be read, or set it to zero if your device does not use numbered reports. |
| size_t                             | **length** | the number of bytes to read, including an extra byte for the report ID. The buffer can be longer than the actual report.                                                                             |

## Return Value

(int) Returns the number of bytes read plus one for the report ID (which is
still in the first byte), or -1 on on failure; call
[SDL_GetError](SDL_GetError)() for more information.

## Remarks

Set the first byte of `data` to the Report ID of the report to be read.
Make sure to allow space for this extra byte in `data`. Upon return, the
first byte will still contain the Report ID, and the report data will start
in data[1].

## Version

This function is available since SDL 3.1.3.

----
[CategoryAPI](CategoryAPI), [CategoryAPIFunction](CategoryAPIFunction), [CategoryHIDAPI](CategoryHIDAPI)

